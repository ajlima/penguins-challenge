# Penguins Challenger

![alt text](https://github.com/ajlima/penguins-challenge/blob/56d2f66d609bd730e8bf4e4dfe798e9884ec8fe7/images/lUK3UmO8yMCSnhiIM63d--1--8oo5w.jpg?raw=true)

### This are the rules of our challenge:
    
  1) The data of this service should be stored in one of following databases: (PostgreSQL, MySQL, MongoDB or Elastic Search);
  2) This service should be deployed on a Docker-compose with 2.0 CPU and 3Gb memory limit, you can use the docker-compose.yml stored on this project as starting point;
  3) Participants can choose any programming language of their choice, the unique restriction is that this service should run on a docker-compose environment;
  4) The people structure should be capable to store all information of Person object;
  5) You must implement the contract described openapi.yml;
  6) This service should be replicated with at least 2 instances;
  7) This environment must have one load-balancer in front of the services and only his IP should be exposed to outside, each request received by this load-balancer must be rounding-robin to each of instance;
  8) All database objects and configuration should be created automatically when this environment is started;
  9) You can distribute the resources as you want, but it is important to say that all records should be persisted on the database that you choose.  It means that you can create a index server, cache server or any other server as you want, but you must observe the hardware limits;
  10) All docker images should be deployed at hub.docker.com;
  11) All code repositories should be stored on Github on a public repository;
  12) The endpoint responsible for the search of all people using a query parameter must execute this search on all fields of Person object, it means that any value used on insert person can be used on this search, including part o this information. Ex: name = Alexandre Lima, if the user inform at query parameter only q=Alex this record should be included in the result;

#### The winner of this challenge will be the participant that create an application capable to process more request/seconds
