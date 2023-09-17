# ADR 2: Travel Management Systems as fallback ?
## Date : 14-09-2023 
## Status
Approved

## Context 
Road Warrior has multiple ways to fetch the travel details , out of which one way is to fetch details from Travel Management Systems[TMS] like SABRE/APOLLO . Agency API's are intially hit to fetch the details of the trip , but when the API's fail to get the data , this TMS interface can be utilized to fetch the travel data of the user for failover mechanism .

## Decision 
We will deploy Agency Failover mechanism by using TMS 

## Consequences
pro's
Get updates even the Agency API's are down
