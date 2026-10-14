# Container Observability

## Nginx Container Setup

I created an Nginx container named `client-website` and mapped port 8080 on the server to port 80 inside the container.

```bash
sudo docker run -d -p 8080:80 --name client-website nginx
```

## Generating Web Traffic

I used the `curl` command to simulate users accessing the website. I sent three requests to the main page and one request to a page that does not exist.

```bash
curl http://localhost:8080
curl http://localhost:8080
curl http://localhost:8080
curl http://localhost:8080/hidden-admin-page
```

The first three requests returned a successful response, while the last request returned a `404 Not Found` response.

## Application Logs

I used the following command to view the requests recorded by the Nginx container.

```bash
sudo docker logs client-website
```

**HTTP 404 Log Entry:**

```
172.17.0.1 - - [14/Oct/2026:00:01:14 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"
```

Application logs are useful because they show the requests received by the web server and the responses returned. They help administrators identify failed requests and investigate possible problems.

## Container Resource Metrics

I used the `docker stats` command to monitor the CPU and memory usage of the Nginx container.

```bash
sudo docker stats --no-stream
```

| Metric | Observed Value |
|---|---|
| Container Name | `client-website` |
| CPU Usage | 0.00% |
| Memory Usage | 2.809 MiB |
| Memory Limit | 1.859 GiB |

These metrics help show how much of the server's resources the container is using at the time of monitoring.

