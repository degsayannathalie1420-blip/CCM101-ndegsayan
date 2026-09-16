# Mission 4 Reflection

## Reflection

Docker containers provide a faster and more lightweight way to deploy applications compared with installing a complete operating system on a Virtual Machine. When using a Virtual Machine, an operating system must be installed and started before the application can be configured. A Docker container can start much faster because it uses the host operating system kernel instead of requiring a complete guest operating system. In this activity, I was able to pull an Nginx image and run a web server using Docker commands.

Port mapping using `-p 8080:80` is necessary because the Nginx web server listens on port 80 inside the container, while port 8080 is the host port used to access the service. The mapping connects port 8080 on the host to port 80 inside the container. This allows a request sent to `localhost:8080` to reach the Nginx web server running inside the container.

When the `docker rm` command is used, the specified container is removed from Docker. Data stored only in the container's writable layer can be lost when the container is removed. This shows why persistent data should be stored using appropriate storage such as Docker volumes when the data needs to remain available after a container is deleted.

Containerization also changes how software developers and IT operations teams work together. Developers can package applications and their dependencies into containers, while operations teams can deploy those containers consistently in different environments. This supports collaboration between development and operations teams and is an important part of DevOps practices.

My GitHub portfolio is evolving as I continue adding organized laboratory activities and technical documentation. Laboratory 04 adds practical experience with Docker, Nginx, containers, command-line operations, and Markdown documentation. Maintaining an organized portfolio allows me to document my progress and demonstrate the cloud computing skills I have developed throughout the course.
