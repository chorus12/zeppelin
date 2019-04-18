# Dockerized quickstart cloudera and zeppelin 0.8.1

The purpose is to run [quickstart cloudera](https://hub.docker.com/r/cloudera/quickstart) along with [zeppelin](https://hub.docker.com/r/apache/zeppelin) integrated to cloudera docker.

For this purpose zeppelin docker is being modified - python2 removed, added python3, removed R-packages.  
The [Dockerfile](https://github.com/chorus12/zeppelin/blob/master/zeppelin/zep/Dockerfile).  
Image is [here](https://cloud.docker.com/u/bodbe/repository/docker/bodbe/zeppelin).  


To run the application:  
1. Run `docker pull bodbe/zeppelin:python3 && docker pull cloudera/quickstart` to get the images from dockerhub  
2. Clone this repo  
3. Edit docker-compose.yml - it contains custom volumes that need to be adjusted
4. Run `docker-compose build`
5. Run `docker-compose up`

**Pay attention** that zeppelin port mapping is **7777:8888** and from the host you acccess zeppelin http://localhost:7777




