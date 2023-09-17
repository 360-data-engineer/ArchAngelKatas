# ADR 2: Travel Management Systems as fallback?
## Date : 14-09-2023 
## Status
Approved

## Context 
The Road Warrior has multiple ways to fetch the travel details, out of which one way is to fetch details from Travel Management Systems[TMS] like SABRE/APOLLO. Agency APIs are initially called to fetch the details of the trip, but when the APIs fail to get the data, this TMS interface can be utilized to fetch the travel data of the user for the failover mechanism.

## Decision 
We will use TMS integration as a failover mechanism.

## Consequences
Pros -
- Can seek updates from TMS when the Agency is down, thus ensuring the seamless functioning of our system.
