# Laboratory 6: The Cloud Deployment Engineer

## Mission Overview

In this laboratory, I worked as a Cloud Deployment Engineer for CloudNova Technologies. The activity focused on moving from manually running individual Docker containers to using Infrastructure as Code with Docker Compose. I deployed a two-tier cloud storage system consisting of Nextcloud as the application and MariaDB as the database.

## Objectives

- Understand how a multi-tier application is organized.
- Learn the basic structure and purpose of a `docker-compose.yml` file.
- Use the `nano` editor to create and modify configuration files.
- Deploy Nextcloud and MariaDB together using Docker Compose.
- Record deployment steps and Infrastructure as Code concepts using Markdown.
- Add the completed laboratory work to my GitHub Cloud Computing portfolio.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
docker-compose up -d
docker-compose ps
docker-compose down

## Screenshots

-screenshots/compose-deployment.png - Shows the containers running successfully after deployment.
-screenshots/nextcloud-web.png - Shows the Nextcloud setup page through the web browser.
-screenshots/compose-teardown.png - Shows the containers after the deployment was stopped and removed.

## Skills Learned

- Understanding and creating a two-tier application setup
- Creating and editing YAML configuration files
- Starting and stopping multiple Docker containers with Docker Compose
- Using environment variables for application configuration
- Understanding service-name communication between containers
- Mapping container ports for web access
- Documenting technical activities using Markdown and Git/GitHub
