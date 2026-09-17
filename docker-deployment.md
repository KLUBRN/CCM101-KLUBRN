# Docker Deployment Log

## Docker Container Management

### 1. Check Running Containers
`docker ps` was used to see the containers that are currently running.

### 2. Stop the Nginx Container
`docker stop my-nginx` was used to stop the Nginx container.

### 3. Check All Containers
`docker ps -a` was used to display all containers, including stopped containers. The `my-nginx` container should now have an `Exited` status.

### 4. Remove the Container
`docker rm my-nginx` was used to remove the stopped Nginx container.

### Summary

These commands demonstrate how to manage a Docker container from running, stopping, checking its status, and removing it when it is no longer needed.

![Container Lifecycle](./screenshots/container-lifecycle.png)
