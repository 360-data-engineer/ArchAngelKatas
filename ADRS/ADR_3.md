# ADR 3:Datalake vs DB : Data storage solution for Analytics & reporting
## Date : 15-09-2023
## Status
Approved

## Context 
Road Warrior must gather analytical data from users trips for various purposes - travel trends, locations, airline and hotel vendor preferences, cancellation and update frequency etc.
A database is a collection of data or information. Databases are typically accessed electronically and are used to support Online Transaction Processing (OLTP)
Data lakes are a cost-effective way to store huge amounts of data. We can use data lake when you want to gain insights into your current and historical data in its raw form without having to transform and move it. Data lakes also support machine learning and predictive analytics.
Data lakes are OLAP systems 


## Decision 
We will deploy Data storage for Analytics & Rerporting 

## Consequences
Pro's:
Easy data storage simplifies ingesting raw data
A schema is applied afterwards to make working with the data easy for business analysts
Separate storage and compute

Con's:
Requires effort to organize and prepare data for use