# ADR 2: API built with C# .Net Core 6.0
# Context
This is an example project where the primary goal is to help people grow and improve their skills as well as help to build their social network within Made Tech.

The team members had identified their learning objectives for this project which play a major role in the architecture decision made.

Many of the team have not delivered software in line with the UK governments Service Manual, as a result another goal of this project is to improve the teams understanding of and challenges that come with delivering software inline with the service manual.

Most of the developers in the project have experience with C#, some have experience with .Net Core (various versions) and others with .Net Framework.

Ruby is popular within Made Tech and NodeJS was another option that was highlighted as a potential option.

which could also be leveraged to create the API but at the time there wasn't enough experience within the team of Ruby so we felt that learning Ruby would become a distraction and slow velocity impacting other non-technical members of the team.

NodeJS was another consideration but few developers had experience of this so it fell into the same category as Ruby.

Serverless was another option, running code within Llamba functions in AWS however there is a learning goal within the team to learn about CI/CD and utilising Serverless would not prevent them from learning some key concepts around CI/CD when deploying to a server.

# Decision
We will use C# .Net Core 6.0 to build the API both because there are learning opportunities in this area for the development team but also because it will allow the team to focus their learning in other areas of the project, such as CI/CD, cloud infrastructure and delivering software in line with the UK Governments Service Manual.

Ruby and NodeJS were not chosen as the development team felt there would be limited support and leadership within the team which would likely impact the team's velocity.

# Status
Accepted.

# Consequences
C# .Net 6.0 Core gives us flexibility over deployment, is widely used, well documented and well supported. It also gives us access to a large number of packages and frameworks that can simplify implementation.

Developers on the project are all familiar with with C# so this should allow for rapid development of the API allowing the development team to focus more on other areas of the project that they have learning goals in, such as CI/CD, architecture, agile development and will enable us to leverage cloud infrastructure.

