# ADR 4: Email Crawler and Email Processor On Client Side Better Over Server Side
## Date 15-09-2023
## Status
Approved

## Context 
When the user gets travel updates, The Road Warrior should notify the user within 5 minutes of update reception. The Road Warrior will fetch travel updates by crawling and processing emails of the user. Here, we have 2 options to crawl emails & deduce travel updates - either we deploy a service at the server end, which will crawl & parse emails for all the 2 million active users. But this will need a highly resilient and highly available server. Or, we can deploy this service at the client end for all the users. This will bring down the complexity to a great extent and will help us scale easily & comfortably.

## Assumptions
Here we assume that the user has given consent to read his/her emails. All the users must have mobile applications installed.

## Decision 
We will deploy Email Crawler and Parser on the client side because this can ensure low latency in notifying the user.

## Consequences
Pros :
- User will get faster updates
- Easily scalable, low-maintenance design
