# Mission 6 Reflection

## 1. Compose vs. Manual Commands

Using a `docker-compose.yml` file is more convenient because the settings for the whole application are kept in one place. Instead of entering several Docker commands every time, I can use Compose to start the same setup with a single command. It also makes the configuration easier to save, share, and manage through GitHub, which is an important part of Infrastructure as Code.

## 2. Indentation Errors in YAML

YAML depends on proper spacing to understand the relationship between different settings. Using incorrect indentation or Tabs can cause Docker Compose to report an error and prevent the deployment from starting. This activity taught me that even small formatting mistakes can affect the entire configuration.

## 3. Why Environment Variables?

Environment variables make it possible to provide configuration values to containers without modifying their images. In this setup, Nextcloud and MariaDB need matching database information, so the required values are defined in the Compose configuration. For an actual production environment, sensitive passwords and other secrets should be stored more securely instead of being placed directly in a public repository.

## 4. Deploying Nextcloud in Minutes

I was surprised by how quickly Nextcloud became available after running the Compose command. It showed me how containers and automation can reduce the amount of manual work needed to set up an application. This makes deployment faster and more consistent.

## 5. Growth Since Mission 1

Since Mission 1, I have moved from learning basic cloud concepts to working with actual containerized services. I have learned about Docker, storage, and multi-container applications using Docker Compose. I now understand that cloud computing also involves designing, deploying, and managing systems through automation and configuration files.
