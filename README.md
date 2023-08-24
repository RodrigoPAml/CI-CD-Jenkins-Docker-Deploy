# Docker-Deploy

Some dockerfiles and scripts to create a complete application with postgres with C# and NextJS Back-End/Front-End running in docker containers

# Database
  - Docker file and compose to setup a postgres database

# Back-end
  - Docker file and compose to setup a c# asp net back-end in the same network as the database

# Front-end
  - Docker file and compose to setup a front-end in nextJS that send requisitions to the back-end API Rest

# Starting Containers

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
