# Laboratory Activity 7: The Cloud Operations Engineer

## Mission Overview

In this laboratory activity, I checked the health of an Ubuntu server and monitored a website running inside a Docker container. I used Linux commands to check system resources, tested the Nginx web server, and examined its logs and performance metrics.

## Objectives

- Check the server's memory, disk space, and CPU activity.
- Deploy an Nginx web server using Docker.
- Generate HTTP requests using the `curl` command.
- Examine container logs and identify a failed request.
- Monitor the CPU and memory usage of the container.
- Document the results and add screenshots to my GitHub portfolio.

## Monitoring Commands Executed

| Command | Purpose |
|---|---|
| `free -h` | Checks RAM and swap usage. |
| `df -h /` | Checks the root filesystem's storage capacity. |
| `top` | Displays CPU activity and running processes. |
| `sudo docker run -d -p 8080:80 --name client-website nginx` | Creates and starts the Nginx container. |
| `curl http://localhost:8080` | Tests access to the website. |
| `curl http://localhost:8080/hidden-admin-page` | Tests a page that should return a 404 response. |
| `sudo docker logs client-website` | Displays the container's logs. |
| `sudo docker stats --no-stream` | Monitors container resource usage. |

## Skills Learned

Through this activity, I learned how to check Linux server resources and monitor a web application running in Docker. I also practiced generating HTTP requests, reading server logs, and checking CPU and memory usage. These skills helped me understand how monitoring information can be used to identify problems and check the condition of a cloud application.
