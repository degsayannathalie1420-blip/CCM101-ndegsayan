# Docker Deployment

## Overview

This document records the Docker commands used to verify the Docker environment, deploy an Nginx web server, and manage the lifecycle of a container in the KillerCoda Playground.

## Check Docker Installation

### Command

docker --version

This command displays the installed Docker version.

### Check Docker Environment

Command

docker info

This command displays detailed information about the Docker environment and its configuration.

### Deploy Nginx

Pull the Nginx Image

docker pull nginx

This command downloads the official Nginx image from Docker Hub.

### Run the Nginx Container

docker run -d --name nginx-server -p 8080:80 nginx

This command creates and starts an Nginx container in detached mode and maps port 8080 on the host to port 80 inside the container.

### Test the Nginx Web Server

curl http://localhost:8080

This command sends an HTTP request to the Nginx web server through port 8080 and verifies that the server is responding.

### Container Lifecycle
1. List Running Containers
docker ps

This command lists the containers that are currently running.

2. Stop the Container
docker stop nginx-server

This command stops the running Nginx container named nginx-server.

3. Verify the Container Status
docker ps -a

This command displays all containers, including stopped containers, so the status of the Nginx container can be verified.

4. Remove the Container
docker rm nginx-server

This command removes the stopped nginx-server container from the Docker environment.

5. Verify the Removal
docker ps -a

This command confirms whether the nginx-server container has been removed.

### Summary

The Docker commands demonstrated the basic lifecycle of a container. The process included checking Docker, downloading an Nginx image, running the container, testing the web server, stopping the container, verifying its status, and removing it.
