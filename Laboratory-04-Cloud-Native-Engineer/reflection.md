# Mission Reflection

In this laboratory, I learned about Docker containers and how they are different from Virtual Machines. When using Docker, the boot time is much faster because the container does not need to install a complete operating system. It only uses the resources and files needed by the application. In a Virtual Machine, we need to install an operating system first, configure it, and setup the web server. This process can take more time compared to running a Docker container.

Port mapping `-p 8080:80` is necessary because it allows users to access the web server inside the container through the host computer. Port 80 is the port used by Nginx inside the container, while port 8080 is the port exposed on the host. Without port mapping, the web server may be running inside the container, but users outside the container cannot easily access it using the host port.

I also learned that when we use the `docker rm` command, the container is permanently removed. The data stored inside the writable layer of that container will also be deleted. Because of this, important files should be saved using volumes or other storage methods so the data will not be lost when the container is removed.

Containerization can change how software developers and IT operations teams work together. Developers can create applications in a similar environment as the operations team. This can reduce problems caused by different configurations and make deployment more easier. It also helps the team work faster and communicate better because they are using the same container setup.

My GitHub portfolio is also evolving because I am adding more laboratory activities, documentation, screenshots, and reflections. Before, my repository was only containing simple files, but now it shows my learning about cloud computing, Docker, and cloud-native engineering. I am becoming more confident in using commands and managing my projects. This laboratory helped me understand that containerization is useful for modern software development and IT operations.
