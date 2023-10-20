# Docker-Deploy

Some jenkinsfiles and dockerfiles with scripts to create a complete application with postgres with C# and NextJS Back-End/Front-End running in docker containers

Can be used to deploy the repositories 
  - https://github.com/RodrigoPAml/BadgesWebsite
  - https://github.com/RodrigoPAml/ASP-NET-Base-project
  - https://github.com/RodrigoPAml/Next-JS-Base-Repo

# Database
  - Docker file and compose to setup a postgres database

# Back-end
  - Docker file and compose to setup a c# asp net back-end in the same network as the database
  - Jenkins file for CI/CD pipeline
  - 
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
