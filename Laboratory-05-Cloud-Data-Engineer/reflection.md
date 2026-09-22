# Mission Reflection

Object storage is a better option for storing millions of photos because it is designed to handle large amounts of data. Block storage divides data into fixed-size blocks and is usually connected to a specific server, making it useful for operating systems and databases. However, managing millions of individual files this way can become difficult and costly. Object storage treats each photo as a separate object with its own metadata and unique identifier, allowing storage capacity to scale easily while files can be accessed through HTTP and APIs.



Docker simplified the process of deploying MinIO because there was no need to manually install and configure the software. With one docker run command, the MinIO image could be downloaded and started, ports 9000 and 9001 could be configured, and the login credentials could be provided through environment variables. This also makes the deployment easier to repeat on other systems that have Docker installed.



A bucket in cloud storage serves as a main container for storing objects. It can be compared to a top-level folder, although it is designed specifically for object storage. Each bucket has a unique name and can have its own access rules and configurations. In this laboratory activity, I created the client-photos bucket to store the photos uploaded by the client.



Large organizations can help protect data from being lost by keeping copies of data across different storage devices, servers, and sometimes different data centers or regions. Methods such as replication and erasure coding can help recover data if a server or storage device fails. Backups and versioning can provide additional protection against accidental deletion or other data problems.



My confidence in using the Linux command line has improved through this activity. Using Docker commands, checking running containers with docker ps, and managing project files with Git have become more familiar to me. Although I still need to check command options from time to time, I now have a better understanding of how the commands work and can handle basic errors more confidently.
