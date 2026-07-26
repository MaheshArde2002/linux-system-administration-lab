# Service Management

## Overview

A service is a background program that runs continuously to perform specific tasks. Linux uses **systemctl** to manage services.

---

## Common Commands

### Check Service Status

```bash
systemctl status nginx
```

Displays the current status of the Nginx service.

---

### Start a Service

```bash
sudo systemctl start nginx
```

Starts the service.

---

### Stop a Service

```bash
sudo systemctl stop nginx
```

Stops the service.

---

### Restart a Service

```bash
sudo systemctl restart nginx
```

Restarts the service.

---

### Reload a Service

```bash
sudo systemctl reload nginx
```

Reloads the configuration without stopping the service.

---

### Enable a Service

```bash
sudo systemctl enable nginx
```

Starts the service automatically after system boot.

---

### Disable a Service

```bash
sudo systemctl disable nginx
```

Prevents the service from starting automatically.

---

### Check if a Service is Active

```bash
systemctl is-active nginx
```

Returns whether the service is running.

---

### List Running Services

```bash
systemctl list-units --type=service
```

Displays all active services.

---

## Commands Practiced

```bash
systemctl status nginx
sudo systemctl start nginx
sudo systemctl stop nginx
sudo systemctl restart nginx
sudo systemctl reload nginx
sudo systemctl enable nginx
sudo systemctl disable nginx
systemctl is-active nginx
systemctl list-units --type=service
```

---

## What I Learned

- Understanding Linux services
- Managing services using systemctl
- Checking service status
- Starting and stopping services
- Enabling services at boot