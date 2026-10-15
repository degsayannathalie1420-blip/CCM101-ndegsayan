# Laboratory 08: The Cloud Security Engineer

## Mission Overview

The purpose of this laboratory is to learn how to protect a cloud server from unauthorized network connections. I deployed an Nginx web application and used UFW to manage the server's firewall. I allowed the required connections while blocking incoming traffic by default.

## Objectives

- Learn basic cloud server security practices.
- Understand why unnecessary ports should be closed.
- Apply a Default Deny firewall policy.
- Allow SSH for server administration.
- Allow port 8080 for the web application.
- Verify and document the firewall configuration.

## Commands Executed

```bash
docker run -d --name secure-web-app -p 8080:80 nginx
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

I learned how to run a web application in a container and protect it using firewall rules. I also learned that opening unnecessary ports can create security risks. Checking the firewall status is important because it helps confirm whether the expected rules are active. This activity improved my understanding of server protection and responsible cloud administration.

## Screenshots

- `screenshots/vulnerable-app-running.png`
- `screenshots/firewall-activated.png`
- `screenshots/firewall-port-allowed.png`
