Cloud9 v3 Dockerfile
=============

This repository contains Dockerfile of Cloud9 IDE for Docker's automated build published to the public Docker Hub Registry.

# Base Docker Image
[dockerfile/supervisor](https://registry.hub.docker.com/u/dockerfile/supervisor/)

# Installation

## Install Docker.

## Build and run with custom config directory

Get the latest version from github

    git clone https://github.com/AshDevFr/docker-cloud9.git
    cd cloud9-docker/

Build it

    sudo docker build --force-rm=true --tag="$USER/cloud9-docker:latest" .
    
And run

    sudo docker run -d -p 8181:8181 -v /your-path/workspace/:/workspace/ $USER/cloud9-docker:latest
    
Enjoy !!    

Thanks to kdelfour (github.com/kdelfour/cloud9-docker)
