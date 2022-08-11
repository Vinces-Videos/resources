# ADR 1: Three tiered architecture

# Context
This is an example project where the primary goal is to help people grow and improve their skills as well as help to build their social network within Made Tech.

The team members had identified their learning objectives for this project which play a major role in the architecture decision made.

The developers on the team have experience of a wide range of different programming languages and frameworks but most come from a C# background and have experience using microservices to deliver distributed systems.

Many of the team have not delivered software in line with the UK governments Service Manual, as a result another goal of this project is to improve the teams understanding of and challenges that come with delivering software inline with the service manual.

# Decision
## Option 1
We decided that the most flexible approach that would help facilitate the team's learning would be to follow the three tiered architecture approach consisting of a presentation tier (web application), an application tier (REST API) and a data tier (SQL Database).

Additionally this would allow more concurrent work streams as developers could work on different tiers simultaneously when working on a user story.
## Option 2
We decided that the API layer and Data layer should live together…

# Status
Pending.

# Consequences
## Option 1
This results in having to manage three separate repositories, for the UI, one for the API and one for the database.
Allows future developers to revisit the project and recreate and integrate any tier they wish using a different technology.

## Option 2

