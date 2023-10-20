# Repository

Some jenkinsfiles and dockerfiles with scripts to create a complete application with postgres, C# and NextJS Back-End/Front-End running in docker containers

Can be used to deploy the repositories 
  - https://github.com/RodrigoPAml/BadgesWebsite
  - https://github.com/RodrigoPAml/ASP-NET-Base-project
  - https://github.com/RodrigoPAml/Next-JS-Base-Repo

## Continuous Integration and Continuous Deployment (CI/CD)

CI/CD stands for Continuous Integration and Continuous Deployment (or Continuous Delivery), and they are practices in software development and DevOps that help automate and streamline the process of building, testing, and deploying software.

**Continuous Integration (CI):**
- Continuous Integration (CI) is a development practice where developers frequently integrate their code changes into a shared repository, typically multiple times a day.
- Each integration triggers an automated build and a set of tests to ensure that the new code doesn't break existing functionality.
- The main goal of CI is to catch and fix integration issues as early as possible, ensuring that the codebase is always in a working state.

**Continuous Deployment (CD):**
- Continuous Deployment (CD) is an extension of CI that involves automating the deployment of code changes to production or staging servers.
- With CD, any code that successfully passes the CI pipeline can be automatically deployed to a testing environment and, if it passes further tests, to production.
- The ultimate goal of CD is to deliver new features, fixes, and updates to end-users as quickly and as frequently as possible.

In summary, CI/CD is a set of practices and tools that promote automation and collaboration in the software development process. It helps reduce manual errors, improves the speed of development, and ensures that software is continually tested and delivered in a more reliable and consistent manner. It's a fundamental part of modern software development and DevOps workflows.

# Database
  - Docker file and compose to setup a postgres database

# Back-end
  - Docker file and compose to setup a c# asp net back-end in the same network as the database
  - Jenkins file for CI/CD pipeline
    
# Front-end
  - Docker file and compose to setup a front-end in nextJS that send requisitions to the back-end API Rest

# Starting Containers local

```
./start_database.sh
./start_back.sh
./start_front.sh
```

# Check Database and Back-End connectivity

Inside the back-end docker bash run (docker exec -it [container-id] bash)

Install depencies if needed

```
  su
  apt update
  apt install ping
```
then

```
  ping postgres
```
