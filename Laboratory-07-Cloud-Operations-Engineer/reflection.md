# Reflection

This laboratory activity helped me understand how to monitor a Linux server and check the condition of a web application running in Docker. I learned that checking an application requires more than just seeing if the website opens. We also need to examine system resources, logs, and performance metrics.

**1. Why is it important to check the host server's resources even if your containers are running perfectly?**
It is important to check the host because containers depend on the server's CPU, memory, and disk space. If these resources become limited, the application may slow down or stop working properly, even if the container was running fine before.

**2. If a user complains that they cannot log into a web application, how would the `docker logs` command help you solve the problem?**
I would use `docker logs` to check the messages recorded by the application. These logs may show errors or failed requests that can help me investigate the login problem and find its possible cause.

**3. What is the difference between monitoring logs and monitoring metrics?**
Logs contain records of events, such as successful requests and errors. Metrics show numerical information, such as CPU usage and memory consumption. Logs help explain what happened, while metrics help monitor the performance and resource usage of the application.

**4. How do you think large enterprise companies monitor thousands of containers at the same time?**
Large companies can use monitoring tools like Prometheus and Grafana. Prometheus collects performance metrics, while Grafana displays the information through dashboards. These tools help technical teams monitor many containers and identify possible issues more easily.

**5. How has your ability to troubleshoot Linux environments improved?**
My troubleshooting skills improved because I learned how to use commands such as `free -h`, `df -h /`, `top`, `docker logs`, and `docker stats`. I can now check system resources, examine application logs, and observe container performance to help identify problems.

Overall, this activity taught me the importance of monitoring and documenting system performance. I can apply these skills to future cloud computing activities and use actual command outputs to support my observations.
