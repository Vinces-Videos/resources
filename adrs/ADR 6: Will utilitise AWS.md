# ADR 6: We will utilitise AWS.

# Context
The goal of this project is to have a publically accessible website for Vinces Video store. We don't own any servers that we could use to host the website on ourselves and we want to be able to host the website without inncuring any unnecessary expense.
Made Tech are also partnered with AWS and Microsoft and many of our deliveries leverage their cloud computing platforms. Addtionally these cloud computing platforms are commonly requested learning resources within Made Tech.
These platforms also support containerisation which is a requirement as a consequence of ADR #5.
All of the developers on the project are currently proceeduing through AWS courses.

# Decision
We chose to host utilitise the AWS cloud computing platform to host the site. 
The main driver behind this decision over using something like Microsoft Azure was that most of the developers are actively learning about AWS.
This was by far the most cost effective means of hosting our site with the expected cost to be less than £1 for the entirity of development. It would mean we would not have to purchase and maintain any of our own servers and would give us a disposable environment for development.

# Status
Accepted.

# Consequences
We must learn how to build the infrastructure we require in AWS and create workflows in GitHub that allows us to deploy the latest changes to AWS.
We must be careful to only use what we require in AWS to incur as little costs as possible - which in turn will limit what features we are able to take advantage of.
Creating the infrastructure and learning to monitor the application in AWS may take longer than we anticipate due to little/no prior knowledge of the platform.
We will need to be strict around who has access to the AWS account as it will be funded by one of the developers personal credit cards.
Eventually we will be able to host the application within the Made Tech AWS sandbox environment so it can be refered to by other developers.
