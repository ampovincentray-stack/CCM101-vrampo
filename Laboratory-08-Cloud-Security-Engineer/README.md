# Laboratory 08: The Cloud Security Engineer

## Mission Overview

The laboratory activity is based on securing an Ubuntu server making use of a host-based firewall. I deployed an Nginx web application on the server using Docker and configured UFW in a way that allows only essential traffic, but blocks any incoming connections.

## Objectives

- Understand the Principle of Least Privilege.
- Explain the attack surface
- Set up a default-deny incoming firewall policy
- Allow SSH and TCP port 8080.
- Verify the firewall rules and test the web application
- Provide documentation of the security settings with Markdown

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

- Deploying a web application in docker
- Testing web applications with the use of curl
- Configuring UFW on Ubuntu.
- Configuring UFW in Ubuntu
- Managing firewall rules
- Applying the Principle of Least Privilege and Default Deny

## Screenshots

- `screenshots/vulnerable-app-running.png`
- `screenshots/firewall-activated.png`
- `screenshots/firewall-port-allowed.png`
