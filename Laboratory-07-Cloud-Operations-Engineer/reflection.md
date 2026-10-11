# Mission 7 Reflection

Before completing this activity, I mainly thought that running a container was the most important part of deploying a web application. After working with the monitoring commands, I understood that checking the condition of the server is also necessary. An application can be running while the host is already experiencing resource problems.

The host resource checks helped me understand the role of memory and storage in maintaining a service. RAM is needed by running processes, while disk space is used for files, logs, and other data. If either resource becomes insufficient, the application may slow down or experience errors. Establishing a baseline also gives an operator something to compare against when investigating later problems.

I also learned that `docker logs` can be useful when a user reports a problem with a web application. By reviewing the recorded requests and errors, an operator can look for clues about what happened. For a login problem, the logs may reveal an application error or a failed request, although additional investigation may be needed if the cause is not recorded there.

Logs and metrics serve different purposes. Logs provide details about events and individual requests, while metrics summarize resource measurements such as CPU usage and memory consumption. Logs can help explain what happened, and metrics can help show whether resource usage may be contributing to the problem.

In larger companies, manually checking every container would be difficult. Monitoring systems such as Prometheus can collect metrics from many services, while Grafana can display the information in dashboards. This allows operations teams to observe trends and investigate unusual activity across their infrastructure.

This activity gave me practice using Linux commands, deploying Nginx with Docker, testing HTTP responses, and examining application logs. It also showed me why technical evidence is important when reporting system conditions. I learned that troubleshooting should involve checking the available information and testing possible causes instead of making assumptions. These skills can help me approach future cloud computing tasks in a more organized way.
