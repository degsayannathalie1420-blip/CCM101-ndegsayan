# Docker Compose Guide

## The Compose File

The `docker-compose.yml` file is used to configure the two main parts of the Nextcloud system. It defines the MariaDB database service and the Nextcloud application service.

## What does the `services:` block do?

The `services:` section contains the containers required by the application. In this setup, the two services are `database` and `app`, and each service has its own image, settings, ports, and environment variables. Docker Compose also creates a network that allows the services to communicate with one another.

## How did the Nextcloud container find the database?

Nextcloud uses the `MYSQL_HOST=database` setting to identify the database server. The word `database` refers to the service name in the Compose file, and Docker Compose automatically connects the name to the correct container through its internal DNS. This means there is no need to manually enter the database container's IP address.

## docker run vs. docker-compose up -d

| `docker run` | `docker-compose up -d` |
|---|---|
| Usually starts one container at a time | Can start multiple services together |
| Configuration is entered through command options | Configuration is stored in a YAML file |
| Network settings may need to be configured manually | Compose creates a network for the services |
| Commands can be repetitive | The setup can be reused and shared easily |

The `-d` option starts the services in detached mode, allowing the containers to continue running in the background while the terminal remains available.
