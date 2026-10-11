# Container Observability Report

## 1. Purpose

This report records the behavior and resource consumption of the Nginx container named `client-website`. The monitoring process includes checking HTTP responses, reviewing application logs, and observing CPU and memory usage.

## 2. HTTP Request Results

Three requests were sent to the Nginx web server.

* **Request 1:** HTTP 200
* **Request 2:** HTTP 200
* **Request 3:** HTTP 200
* **Missing-page request:** HTTP 404

The HTTP 200 responses indicate that the requested pages were served successfully. The HTTP 404 response shows that the requested path was not available on the server.

## 3. Log Investigation

**Exact log entry for the missing page:**

```text
<html>
<head><title>404 Not Found</title></head>
<body>
<center><h1>404 Not Found</h1></center>
<hr><center>nginx/1.31.6</center>
</body>
</html>```

Application logs help engineers investigate incidents by recording requests and their results. Reviewing these records can reveal error patterns and provide clues about what needs to be checked next.

## 4. Container Resource Metrics

The `docker stats` command was used to inspect the live resource consumption of the container.

* **Container Name:** `client-website`
* **Memory Usage:** 2.738MiB
* **CPU Percentage:** 0.00%

These readings describe the container's resource consumption at the time of measurement. They should be interpreted as a snapshot rather than a guarantee of how the container will behave under heavy traffic.

## 5. Evidence

* `screenshots/install-nginx.png`
* `screenshots/simulation1.png`
* `screenshots/simulation2.png`
* `screenshots/docker-logs.png`
* `screenshots/container-metrics.png`

## 6. Summary

The HTTP tests confirmed successful responses and an intentional missing-page error. Reviewing the logs helps explain the requests, while Docker statistics show how much CPU and memory the container used during the observation.
