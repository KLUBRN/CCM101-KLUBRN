# Laboratory 4: Cloud-Native Engineer

## Mission Overview

This laboratory is about learning cloud-native engineering and containerization using Docker in KillerCoda Playground. In this laboratory, we deployed an Nginx web server inside a Docker container. This help us understand how containers can make application deployment more faster and easier compared to using traditional Virtual Machines.

## Objectives

- To understand the difference between Virtual Machines and Containers.
- To use Docker environment in KillerCoda.
- To practice basic Docker CLI commands.
- To pull and run an Nginx Docker image.
- To learn how to manage Docker containers.
- To create a documentation using Markdown.
- To add and organize the laboratory in GitHub Cloud Computing Portfolio.

## Docker Commands Executed

### Checkpoint 3 — Verifying Docker

- `docker --version` — This command check if Docker is installed and show the Docker version.
- `docker info` — This command displays the information about the Docker environment and Docker daemon.

### Checkpoint 4 — Deploying Nginx

- `docker pull nginx` — This command downloads the Nginx image from Docker Hub.
- `docker run -d -p 8080:80 --name my-nginx nginx` — This command create and run the Nginx container in detached mode.
- `curl http://localhost:8080` — This command is used to test if the Nginx web server is working correctly.

### Checkpoint 5 — Container Lifecycle

- `docker ps` — This command show the containers that is currently running.
- `docker stop my-nginx` — This command stop the Nginx container.
- `docker ps -a` — This command show all containers including the stopped containers.
- `docker rm my-nginx` — This command remove the stopped Nginx container.

## VM vs. Containers

Virtual Machines needs a complete operating system to run, so it can use more resources and takes more time to start. Containers are more lightweight because they share the host operating system. Because of this, containers can start faster and use less resources.

## Skills Learned

- Understanding the difference between Virtual Machines and containers.
- Using basic Docker commands.
- Pulling images from Docker Hub.
- Running an Nginx container.
- Understanding the port mapping.
- Managing the Docker container lifecycle.
- Creating technical documentation using Markdown.

## Challenges Encountered

One challenge I encountered in this laboratory was understanding the port mapping when running the Nginx container. At first, I was confused about the `-p 8080:80` because I was not sure which port is for the host and which one is for the container. I learned that port 8080 is the host port and port 80 is the container port. After understanding this, I was able to access the Nginx web server using `curl http://localhost:8080`.

## Mission Reflection

In this laboratory, I learned more about how Docker containers is being used in cloud-native environment. I learned that containers are lightweight and can start faster because it does not need a complete operating system. I also learned how to pull an image, run a container, check the container status, stop the container, and remove it using Docker commands.

## Conclusion

Laboratory 4 gave me a hands-on experience about Docker and containerized applications. By deploying and managing an Nginx container, I understand better how containerization works and why it is useful in cloud-native infrastructure. This laboratory also helped me become more familiar with using Docker CLI commands.
