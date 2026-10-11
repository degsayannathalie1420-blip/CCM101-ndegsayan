# Mission 7: The Cloud Operations Engineer

## Mission Overview

This activity introduces basic cloud operations and application monitoring. A Linux host was examined before an Nginx web server was deployed through Docker. Test requests were then sent to the server, and its logs and resource statistics were reviewed to understand its behavior.

## Objectives

* Examine the host's memory and disk capacity.
* Observe processes and CPU activity using Linux tools.
* Deploy an Nginx container named `client-website`.
* Test successful web requests and generate a 404 response.
* Review application logs to identify request errors.
* Observe CPU and memory usage with Docker statistics.
* Maintain technical documentation and evidence in GitHub.

## Monitoring Commands Executed

| Command                                                | Purpose                            |
| ------------------------------------------------------ | ---------------------------------- |
| `free -h`                                              | Inspect memory and swap usage      |
| `df -h /`                                              | Check root filesystem capacity     |
| `top`                                                  | Observe processes and CPU activity |
| `docker ps`                                            | Verify running containers          |
| `docker run -d --name client-website -p 8080:80 nginx` | Launch Nginx                       |
| `curl`                                                 | Test web server responses          |
| `docker logs client-website`                           | Review application logs            |
| `docker stats`                                         | Observe live container metrics     |

## Skills Learned

This activity provided practical experience with Linux resource checks, Docker deployment, HTTP testing, and application troubleshooting. It also demonstrated how to document system measurements and monitoring results in Markdown.

## Evidence

The `screenshots/` directory is intended to contain the memory check, disk check, container deployment, HTTP tests, application logs, and Docker metrics.

## Conclusion

A reliable web service requires more than a successful deployment. Checking host resources, reviewing request logs, and observing container metrics gives an operator useful information for identifying errors and evaluating application health.
