# Laboratory 08: The Cloud Security Engineer

## Mission Overview

This laboratory focuses on securing an Ubuntu server using a host-based firewall. I deployed an Nginx web application using Docker and configured UFW to allow required network traffic while denying incoming connections by default.

## Objectives

- Understand the Principle of Least Privilege.
- Explain the concept of an attack surface.
- Configure a default-deny incoming firewall policy.
- Allow SSH and TCP port 8080.
- Verify firewall rules and test the web application.
- Document the security configuration using Markdown.

## Commands Executed

```bash
docker --version
docker run -d --name secure-web-app -p 8080:80 nginx
docker ps
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

- Deploying a web server with Docker.
- Testing a web application with curl.
- Configuring UFW on Ubuntu.
- Managing firewall rules and network ports.
- Applying the Principle of Least Privilege and Default Deny.
- Creating technical documentation and evidence in GitHub.

## Screenshots

- `screenshots/vulnerable-app-running.png`
- `screenshots/firewall-activated.png`
- `screenshots/firewall-port-allowed.png`
