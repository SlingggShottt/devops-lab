# Docker and Jenkins CI integration 

# base image of jenkins
FROM jenkins/jenkins:lts

# switch to root user to install docker
USER root

# install docker inside docker container
RUN apt-get update && apt-get install -y docker.io

# switch back to jenkins user
USER jenkins