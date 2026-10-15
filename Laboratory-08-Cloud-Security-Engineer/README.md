# Laboratory Activity 8: The Cloud Security Engineer

## Mission Overview

For this mission, I worked on securing a Linux server by setting up a firewall and controlling which network connections were allowed. I started an Nginx web application using Docker, then configured UFW to protect the server while keeping the required services accessible. This activity helped me understand how basic security settings can prevent unwanted access.

## Objectives

* Learn about the Principle of Least Privilege and the attack surface.
* Check the network ports and services running on a Linux server.
* Configure UFW to block incoming traffic by default.
* Allow SSH and port 8080 while restricting other incoming connections.
* Record firewall commands and security practices using Markdown.
* Add the completed activity to my GitHub cloud computing portfolio.

## Commands Executed

```bash
sudo docker run -d -p 8080:80 --name secure-web-app nginx
curl http://localhost:8080
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
sudo ufw allow 8080/tcp
sudo ufw status numbered
```

## Skills Learned

In this activity, I practiced running a web server with Docker and setting up firewall rules in Linux. I learned how to restrict incoming connections while allowing the services needed by the application. I also understood why administrators should check open ports and avoid leaving unnecessary services accessible. These skills can help me manage cloud servers more safely in future activities.
