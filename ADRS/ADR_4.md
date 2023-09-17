# ADR 4:Email Crawler and Email Processor On Client Side Better Over Server Side
## Date 15-09-2023
## Status
Approved

## Context 
When the user get travel updates , Road Warrior should notify user within 5 minutes of time .Road Warrior will fetch travel updates by crawling and processing emails of user.Here we have 2 options to fetch travel  updates either we can deploy a service at server end which will continuously poll for all the 2 million active users to fetch details this will need highly resilient and higly available server or we can deploy this service at client end for all the users .

## Assumptions
Here we assume that the user have given consent to read his/her emails.All the users must have mobile applications installed.


## Decision 
We will deploy Email Cralwers and Processors on client side because this can ensure low latency in notifying the user.

## Consequences
Pro's  :
1)User will get faster updates 

Con's :
1)Doesn't work for user who only uses web application