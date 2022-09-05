# ADR 1: Layered architecture

# Context
This is an example project where the primary goal is to help people grow and improve their skills as well as help to build their social network within Made Tech.

The team members had identified their learning objectives for this project which play a major role in the architecture decision made.

The developers on the team have experience of a wide range of different programming languages and frameworks but most come from a C# background and have experience using microservices to deliver distributed systems.

Many of the team have not delivered software in line with the UK governments Service Manual, as a result another goal of this project is to improve the teams understanding of and challenges that come with delivering software inline with the service manual.

# Decision
We decided that the most flexible approach that would help facilitate the team's learning would be to follow the three tiered layered architecture approach consisting of a presentation tier (web application), a business layer (REST API) and a data tier (SQL Database).

Additionally this would allow more concurrent work streams as developers could work on different tiers simultaneously when working on a user story.

The Layered pattern also lends itself to high testability and high ease of development as this pattern is well known and not overly complex to implement.

# Status
Accepted.

# Consequences
This results in having to manage three separate repositories, for the UI, one for the API and one for the database.
Allows future developers to revisit the project and recreate and integrate any tier they wish using a different technology.
The complexity is low providing, making it easy to pick up and learn.
This pattern is one of the most widely adopted patterns thus provides a solid base of learning for those new to software development and can be easily picked up by experienced developers.
