
# ADR 1: Microservices Architecture 
## Date : 14-09-2023 
## Status
Accepted

## Context 
Microservices incorporate the principles of Domain Driven Design which were also originally conceived for solving problems associated with technology-partitioned layered monoliths. The implication is that even if we decide to build the system as a modular monolith, we can still apply the proposed architecture when designing and constructing its individual components. The modular structure of the system should at all times mirror the overall architecture proposed here, at each layer.


## Decision 
We will use the Microservices architecture to model the Road Warrior system

## Consequences
Pros -
- Allows us to separate heavily used components into their own processes to allow them to scale
- Clearly identifies the Domain model and partitioning of the system.

Cons -
- Data and code duplication
- Difficult to execute quickly if we strictly adhere to the architecture and develop each microservice from scratch

