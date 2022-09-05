# ADR 5: We will utilitise Containers.

# Context
One of the aims of this project is to be used as a reference point for other developers. For that reason it is important that the project easy to setup for local development.

# Decision
We chose to containerize each layer of the application using Docker.

Containerisation, while adding another layer of complexity, makes setting up local development environments trivial. Containerisation is also a commom technique in mordern software development and has a relatively low barrier to entry. For those familiar with this technique they will be able to spin up their local environment in just a few minutes and for those new to the technique it will encourage them to learn the basics and reinforce their learning.

We chose to use Docker because several of the team members at the time had experience of using this tool and could provide support where needed to other members of the team. Additionally Docker is one of the most popular containerisation technologies, as a result there is an abundance of online guides, tutorials and support available.

# Status
Accepted.

# Consequences
We must ensure the technology choices across the three layers of the architecture can be easily containerised.
We must ensure that we provide local environment setup instructions that can be followed by a developer that is not familiar with Docker.
This will add an additional layer of complexity into communication between our application tiers.
This will somewhat restrict our deployment options as target servers will need to be able to run Docker.
