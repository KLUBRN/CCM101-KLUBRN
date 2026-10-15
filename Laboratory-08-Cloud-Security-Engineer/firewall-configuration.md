# Firewall Configuration

## Allow SSH

```bash
sudo ufw allow ssh
```

This rule permits SSH connections so administrators can access and manage the server remotely.

## Default Deny Policy

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

These settings block incoming connections unless a rule allows them, while still permitting the server to send outgoing traffic.

## Allow Port 8080

```bash
sudo ufw allow 8080/tcp
```

This rule allows TCP traffic through port 8080 so users can access the web application running on the server.

## What happens if you run sudo ufw enable before sudo ufw allow ssh?

Enabling the firewall before allowing SSH may block remote administration and prevent me from accessing the server through an SSH connection.
