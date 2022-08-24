This outlines the deployment steps, decisions and justifications to deploy the Vinces Videos API. It's worth noting that this does not take into account database or front-end deployment.

For ease of deployment, the entire API is containerised. Having this within a container means that we can have the flexibility to deploy to a number of platforms without having to install .NET onto each. Pretty much all cloud platforms have a way to host containerised applications so they're fairly easy to deploy to them too.

## Technology
The techonologies used for deployment

### Github Actions
This is responsible for taking the source code, then building the solution into a published package. Github Actions will also use pre-configured Amazon Web Services (which are specified within the deploy-to-aws.yml file) to deploy the built solution to Amazon Web Services, where it will eventually end up as an EC2 instance. Fargate was another option for this but has costs associated.

### Docker
Used as our containerisation software, it's very quick and easy to use and has incredible integration, support and documentation. As a first step when building the container, we install .NET and publish the package within the container. 

### Amazon Web Services
A couple of AWS services are used for deployment. 

#### ECS
The service configuration which builds the EC2 based upon the container stored within the elastic container repository.

#### ECR
Github builds an image and posts it to the elastric container repository for usage by ECS

#### EC2
The docker container ends up housed within an EC2 Instance