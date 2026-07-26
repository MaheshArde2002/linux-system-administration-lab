# SSH (Secure Shell)

## Overview

SSH (Secure Shell) is a secure protocol used to connect to a remote Linux server. It allows administrators to manage servers from another computer using the command line.

---

## Common Commands

### Check SSH Service Status

```bash
sudo systemctl status ssh
```

Displays whether the SSH service is running.

---

### Start SSH Service

```bash
sudo systemctl start ssh
```

Starts the SSH service.

---

### Stop SSH Service

```bash
sudo systemctl stop ssh
```

Stops the SSH service.

---

### Restart SSH Service

```bash
sudo systemctl restart ssh
```

Restarts the SSH service.

---

### Enable SSH Service

```bash
sudo systemctl enable ssh
```

Starts the SSH service automatically after system boot.

---

### Connect to a Remote Server

```bash
ssh username@server-ip
```

Example:

```bash
ssh mahesh@192.168.1.100
```

This command connects to a remote Linux server.

---

### Check SSH Version

```bash
ssh -V
```

Displays the installed SSH version.

---

## Commands Practiced

```bash
sudo systemctl status ssh
sudo systemctl start ssh
sudo systemctl restart ssh
sudo systemctl enable ssh
ssh -V
ssh username@server-ip
```

---

## What I Learned

- What SSH is
- How to check the SSH service
- How to start and restart SSH
- How to enable SSH at boot
- How to connect to a remote Linux server

---

## Conclusion

In this lab, I learned the basics of SSH. I practiced managing the SSH service and learned how to connect to a remote Linux server securely.
