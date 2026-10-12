# Firewall Configuration

## Allow SSH

```bash
sudo ufw allow ssh
```

## Default Deny Policy

```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

## Allow Port 8080

```bash
sudo ufw allow 8080/tcp
```

## What would happen if `sudo ufw enable` ran before `sudo ufw allow ssh`?

If I enabled the firewall before allowing SSH, the default deny rule would block all incoming connections, including SSH, and I would be locked out of my own server.
