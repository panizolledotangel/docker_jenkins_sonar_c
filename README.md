# Overview

Docker container to run jenkins and sonarcloud on c projects

# How to run

1. Create environment variables UID and GID with the user id and group id for folder permissions.
```
export UID=`id -u`
export GID=`id -g`
```
2. Build the image.
```
docker compose build jenkins
```
3. Initialize the jenkins service
```
docker compose up 
```
5. The frist time the service is intialized needs to be configured. Follow the instructions in *configure_jenkins.pdf* to do this step.
