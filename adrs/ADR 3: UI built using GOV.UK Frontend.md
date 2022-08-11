# ADR 3: UI built using GOV.UK Frontend

# Context
This is an example project where the primary goal is to help people grow and improve their skills as well as help to build their social network within Made Tech.

The team members had identified their learning objectives for this project which play a major role in the architecture decision made.

Many of the team have not delivered software in line with the UK governments Service Manual, as a result another goal of this project is to improve the teams understanding of and challenges that come with delivering software inline with the service manual.

Most of the team were keen to constrain the project by following the service manual.

# Decision

We will use the GOV.UK Frontend which contains the code needed to start building a user interface for government platforms and services.
# Status
Accepted.

# Consequences
The government service manual specifies that when designing a web page it must consider the case that JavaScript or CSS is disabled or unavailable to the user. For that reason we must consider carefully what front-end frameworks we choose to use in addition to GOV.UK Front - if any.
