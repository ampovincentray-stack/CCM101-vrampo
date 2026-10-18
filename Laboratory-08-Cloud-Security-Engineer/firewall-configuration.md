# Firewall Configuration

## 1. Allow SSH

Command:

```bash
sudo ufw allow ssh
```

Explanation: The regulation allows for SSH connections which enable the users to manage the server from any remote location.

## 2. Configure the Default Policies

Deny incoming traffic by default:

```bash
sudo ufw default deny incoming
```

Allow outgoing traffic by default:

```bash
sudo ufw default allow outgoing
```

Enable the firewall:

```bash
sudo ufw enable
```

Verify the configuration:

```bash
sudo ufw status verbose
```

Explanation: Under the condition of a default-deny incoming regulation, all connections will get blocked unless there is any prior authorization given so that a connection can be made. However, outgoing connections will be enabled as a default.


## 3. Allow the Web Application

Command:

```bash
sudo ufw allow 8080/tcp
```

Verify the rules:

```bash
sudo ufw status numbered
```

Test the application:

```bash
curl http://localhost:8080
```

Explanation: The TCP port 8080 regulation allows connections to come to the port of the web application that is published.

## 4. Why SSH Must Be Allowed Before Enabling UFW

If the command sudo ufw enable is issued before issuing the command sudo ufw allow ssh, the SSH connection of the remote administrator will be blocked, thus causing the administrator to be locked out from the server.

## 5. Security Best Practices

- Permit the entry of necessary ports only.
- Use the default-deny incoming policy.
- Confirm the firewall rules after the changes are made.
- Stay away from exposing administrative services to unnecessary networks.
- Regularly monitor the firewall rules.
