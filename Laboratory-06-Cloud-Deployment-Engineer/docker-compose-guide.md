# Docker Compose Guide

## What does the services: block do?
The services: block specifies the containers needed to run an application. In this project, it defines the Nextcloud app and the database, including the images and configurations each container needs.

## How does the Nextcloud app find the database?
The Nextcloud container uses the MYSQL_HOST=database setting to locate the database. The name database matches the database service defined in the Compose file, allowing the two containers to communicate over Docker's network.

## Difference between docker run and docker-compose up -d
The docker run command is used to start a container by entering its configuration options directly in the terminal. In comparison, docker-compose up -d reads the configuration from a YAML file and starts the services defined in it together. The -d option runs the containers in the background so the terminal remains available for other commands.
