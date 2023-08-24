# Docker-Deploy

Some dockerfiles and scripts to create postgres with C# and NextJS Back-End/Front-End

# database
  - Docker file and compose to setup a postgres database

# back-end
  - Docker file and compose to setup a c# asp net back-end in the same network as the database

# front-end
  - Docker file and compose to setup a front-end in nextJS that send requisitions to the back-end API Rest

# Starting Containers

```
./start_database.sh
./start_back_end.sh
./start_front_end.sh
```
