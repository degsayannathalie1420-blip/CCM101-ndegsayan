# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A two-tier architecture divides an application into two main parts that communicate with each other through a network. In this activity, the two parts are the Nextcloud application and the MariaDB database.

## The Web/Application Tier

The web/application tier is responsible for interacting with the users. It receives requests from the browser, displays the application, processes actions such as login and file uploads, and communicates with the database when information is needed. In this laboratory, the Nextcloud container serves as the web/application tier.

## The Database Tier

The database tier is responsible for storing information that needs to remain available, including user accounts, login information, and file-related data. It receives requests from the application and sends the required information back. In this laboratory, MariaDB is used as the database container.

## Why Separate Them?

Keeping the application and database in separate containers makes the system easier to manage and maintain. Each container can be restarted, updated, or secured independently, while separating their responsibilities also makes troubleshooting easier and prevents the database from being directly exposed to users.
