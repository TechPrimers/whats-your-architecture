# Challenge 1 - Design a Food Store for FoodiE

# Table of Contents
- [Problem Statement](#problem-statement)
    - [Assumptions](#assumptions)
    - [Things to consider](#things-to-consider)
- [Solutions from Community](#solutions-from-community)

# Problem Statement
You are the Architect for a new restaurant data processing team in a food startup which receives files from different restaurants and third party gateways for the next day's food menu. For ease of use, let call the data store as `Food Store` and the startup's name as `FoodiE`
`Food Store` is the central food repository for all systems in `FoodiE`. 

Create a -
- scalable, extendable, fault tolerant and highly available system for the `Food Store`
- data repository for exposing the restaurant information for consuming applications within `FoodiE`. Eg, `FoodiE UI` (Mobile & Web) applications shall retrieve restaurant and food information from `Food Store`.
- historical store for audit purposes (with old restaurant and food data).

## Assumptions
- Assume the feed from the restaurants/third party gateways can change for restuarant to restaurant. Some restaurants send Start of day files, some expose APIs, some pushes messages via a queueing system (like Kafka/ActiveMQ), etc.,.
- Assume the format sent by these restaurants are not the same.
- Some of the restaurants can send realtime updates on the food menu (via queueing systems)
- You can chose any medium of communication between `Food Store` and internal components in the startup (eg, UI, Reviews, etc).

## Things to consider
- You can leverage any non-Cloud platforms or Cloud Platforms (eg, AWS, Azure or GCP) to overlay your deployment diagram and leverage features from these platforms.

# Solutions from Community
Name      |   Solution      | Comments 
----      | ----            | ----
Adhithyan Sridhar | [Solution](./AdhithyanSridhar.md) | Uses generic architecture with Spring and Elatic ecosystems
Swapnil Chaudari | [Solution](./SwapnilChaudari.md) | This architecture uses AWS resources using mix of Serverless and non-Serverless resources
