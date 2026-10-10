# Laboratory Activity 6: The Cloud Deployment Engineer

## Mission Overview

The goal of this laboratory activity was to deploy a multi-tier application using Docker Compose. I learned how to configure and run Nextcloud with a database container and how to manage the deployment using Linux commands and a YAML configuration file.

## Objectives
Explain the concept of a multi-tier application architecture
Understand the purpose and structure of a docker-compose.yml file
Use a Linux command-line text editor (nano) to create configuration files
Deploy a multi-container application (Nextcloud + Database) using Docker Compose
Document deployment procedures and Infrastructure as Code (IaC) principles using Markdown
Continue expanding your professional GitHub Cloud Computing Portfolio
## Commands Executed
mkdir nextcloud-deployment – Creates a directory for the deployment project.
cd nextcloud-deployment – Moves into the project directory.
nano docker-compose.yml – Creates or edits the Docker Compose configuration file.
sudo docker-compose up -d – Starts the application and database containers in the background.
sudo docker-compose ps – Checks the status of the containers.
sudo docker-compose down – Stops and removes the containers and network created by Docker Compose.

## Skills Learned

Through this activity, I learned how to use Docker Compose to deploy and manage multiple containers as one application. I also practiced using Linux commands, editing YAML configuration files with nano, and checking container status. This activity helped me understand Infrastructure as Code (IaC) and how configuration files make deployments easier to organize, repeat, and maintain.
