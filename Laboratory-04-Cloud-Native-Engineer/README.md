# Laboratory 04 — Cloud-Native Engineer

## Mission Overview

Laboratory 04 introduces the shift from traditional Virtual Machines to containerization. In this activity, I used the KillerCoda Playground to work with Docker, deploy an Nginx web server, and practice basic container lifecycle operations.

The activity focused on understanding the differences between Virtual Machines and containers and applying Docker commands to pull, run, test, stop, and remove a containerized application.

## Objectives

At the end of this laboratory activity, I was able to:

- Differentiate between traditional Virtual Machines and containers.
- Access a Docker-enabled cloud environment using KillerCoda.
- Execute fundamental Docker CLI commands.
- Pull and run an Nginx container.
- Map a host port to a container port.
- Test a containerized web server.
- Stop and remove a Docker container.
- Document container operations using Markdown.
- Organize technical work in my GitHub Cloud Computing portfolio.

## Docker Commands Executed

### Docker Verification


docker --version

Displays the installed Docker version.

docker info

Displays information about the Docker environment.

### Nginx Deployment

docker pull nginx

Downloads the official Nginx image from Docker Hub.

docker run -d --name nginx-server -p 8080:80 nginx

Runs the Nginx container in detached mode and maps host port 8080 to container port 80.

curl http://localhost:8080

Tests the Nginx web server through the mapped host port.

### Container Lifecycle

docker ps

Lists currently running containers.

docker stop nginx-server

Stops the Nginx container.

docker ps -a

Lists all containers, including stopped containers.

docker rm nginx-server

Removes the stopped Nginx container.

docker ps -a

Verifies the container removal.

### Skills Learned

Through this laboratory activity, I learned how to:

Compare Virtual Machines and containers.
Use the Docker command-line interface.
Pull images from Docker Hub.
Run a containerized application.
Use port mapping to expose a containerized web server.
Test an Nginx web server using curl.
Manage the lifecycle of a Docker container.
Create technical documentation using Markdown.
Organize cloud computing laboratory work in GitHub.

### Challenges Encountered

One challenge was becoming familiar with Docker commands and understanding the difference between an image and a running container. Another challenge was understanding how port mapping connects the host port to the port used by the Nginx service inside the container. The activity also required careful execution of the container lifecycle commands because the container had to be stopped before it could be removed.
