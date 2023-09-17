# O'Reilly Architectural Katas 2023
#### Team ArchAngelKatas
- Gopi Krishna
- K S Sreenidhi
- Shanmukh Gajula
- Abhishek Gupta
- Sagar Kesariya

# The Road Warrior - An Itinerary Management Startup
## Introduction
The Road Warrior wants to build the next-generation online trip management dashboard to allow travelers to see all of their existing reservations organized by trip either online (web) or through their mobile device.

## Requirements
- Poll email looking for travel-related emails
- Filter and whitelist certain emails
- The system must interface with the agency’s existing airline, hotel, and car rental interface system to update travel details (delays, cancellations, updates, gate changes, etc.).
- Updates must be in the app within 5 minutes of an update (better than the competition)
- Customers should be able to add, update, or delete existing reservations manually as well.
- Items in the dashboard should be able to be grouped by trip, and once the trip is complete, the items should automatically be removed from the dashboard.
- Users should also be able to share their trip information by interfacing with standard social media sites or allowing targeted people to view your trip.
- Richest user interface possible across all deployment platforms
- Provide end-of-year summary reports for users with a wide range of metrics about their travel usage
- Road Warrior gathers analytical data from users' trips for various purposes - travel trends, locations, airline and hotel vendor preferences, cancellation and update frequency, and so on.

## User Journey
The following flowchart describes a user's journey end-to-end covering major features. 

While the user signs up, we will be considering the email used as the email ID that's associated with all trips booked online and we seek a one-time consent for email inbox crawling. The user can always choose to enable/disable the email crawl access via the Profile section on the app. 
In case, the email ID used during sign-up isn't associated with a particular booking, then the user can always forward such booking-related updates to The Road Warrior's inbox for further processing and itinerary updates.
We also accommodate complete, end-to-end manual itinerary creation by the user.
![user_journey](/Diagrams/user_journey.png)
*Figure 1 User Journey*

## Architecture Walkthrough
The Road Warrior has been designed by adopting Microservices Architecture (as discussed in the /ADRS/ADR_1_microservices.md). 
The choice of containers & their services mapping have been done basis the actor-actions approach.
We have two actors - The user and the system. 
Their actions have been described in the image below.
![actors_actions](/Diagrams/actors_actions.png)
*Figure 2 Actors-Actions Mapping*

The high-level diagram of server-client interaction via Containers has been attached below. 
![high_level_arch](/Diagrams/high_level.png)
*Figure 3 Server-Client Interaction via Containers*

The low-level diagram explaining the client-server interaction via Containers' services has been attached below.
![architecture](/Diagrams/architecture.png)
*Figure 4 Server-Client Interaction via Services*
