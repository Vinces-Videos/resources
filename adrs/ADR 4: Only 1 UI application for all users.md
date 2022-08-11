# ADR 4: Only 1 UI application for all users

# Context
At this stage of the project we’re aiming to deliver the most valuable product (MVP) only.
There are two main users for this project, staff of the video store (Vincent) and customers of the store.
Vincent wants to be able to retain his ability to serve customers in person within the store itself.
Vincent will require more functionality than his customers, he will need to be able to maintain his stock, create invoices as well the ability to capture and manage customer information.

# Decision
We chose to build a single UI for the sake of the MVP. 

We discussed that there was an opportunity to develop a separate UI for Vincent and his staff but felt because they could be performing the act of renting a video in behalf of the customer that it would make more sense in the context of the MVP to develop a single UI application with the view that a second application could be created, if required, at a later stage.

# Status
Accepted.

# Consequences
Developers will only have to develop, and deploy a single UI Application additionally they  will not need to duplicate models or create a shared library for both of the UI applications and will have less dependencies to manage and less to set up for their local development environment.

We will need a means of authenticating Vincent and his staff (as this is an example project this can be as simple as an admin password).

Developers may encounter conflicts when working on related functionality.
