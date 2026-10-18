# Firewall Configuration

## 1. Allow SSH

Command:

```bash
sudo ufw allow ssh
```

Explanation: This rule permits SSH traffic so administrators can remotely manage the server.

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

Explanation: The default-deny incoming policy blocks connections unless an explicit rule permits them, while outgoing connections are allowed by default.

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

Explanation: The TCP port 8080 rule permits incoming traffic for the web application's published port.

## 4. Why SSH Must Be Allowed Before Enabling UFW

If `sudo ufw enable` is run before `sudo ufw allow ssh`, a remote administrator's SSH connection may be blocked by the default-deny incoming policy, potentially locking the administrator out of the server.

## 5. Security Best Practices

- Allow only the network ports required by the application.
- Use a default-deny incoming policy.
- Verify firewall rules after making changes.
- Avoid exposing administrative services to unnecessary networks.
- Review firewall rules regularly.
