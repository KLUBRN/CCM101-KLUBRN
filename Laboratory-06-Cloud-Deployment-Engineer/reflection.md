# Laboratory Activity 6: Reflection Questions

1. How does a docker-compose.yml file make a cloud engineer’s job easier than manually typing commands?

A docker-compose.yml file makes a cloud engineer’s job easier because it stores all the configurations needed to run an application in one place. Instead of typing long commands for every container, the engineer can use Docker Compose to start multiple services together. It also makes deployments easier to repeat, manage, and share with other team members.

2. What happens if you use a Tab instead of Spaces in a YAML file?

Using a Tab instead of Spaces for indentation in a YAML file can cause a parsing error because YAML requires spaces for indentation. If the file has incorrect formatting, Docker Compose may fail to read the configuration, preventing the containers from starting properly. This is why proper indentation is important when writing YAML files.

3. Why use environment variables like MYSQL_PASSWORD in the Compose file?

Environment variables such as MYSQL_PASSWORD allow the application to receive important configuration values without placing them directly in the application code. They help configure database credentials and other settings more conveniently. However, passwords should be protected, and sensitive values should ideally be stored in environment files that are not committed to public repositories or managed through secrets.

4. How did it feel to deploy Nextcloud in just a few minutes?

Deploying Nextcloud in just a few minutes felt exciting and satisfying because I was able to run a complete application using only a few commands. I realized that Docker Compose saves time and makes deploying applications much simpler. It also gave me more confidence in using Linux commands and managing containers.

5. How has your understanding of cloud computing evolved since Mission 1?

Since Mission 1, my understanding of cloud computing has improved from learning basic concepts to gaining practical experience with deployment tools. I now understand how containers, databases, and application services work together. I also learned that automation and Infrastructure as Code are important because they make cloud deployments more organized, consistent, and easier to maintain.
