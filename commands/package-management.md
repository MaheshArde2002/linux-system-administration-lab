# Package Management

## Overview

Package management is used to install, update, remove, and manage software on Ubuntu Linux. Ubuntu uses the **APT (Advanced Package Tool)** package manager.

---

## Common Commands

### Update Package List

```bash
sudo apt update
```

Updates the package list from Ubuntu repositories.

---

### Upgrade Installed Packages

```bash
sudo apt upgrade -y
```

Upgrades all installed packages to the latest version.

---

### Install a Package

```bash
sudo apt install nginx
```

Installs the Nginx web server.

---

### Search for a Package

```bash
apt search nginx
```

Searches for a package in the repository.

---

### View Package Information

```bash
apt show nginx
```

Displays information about a package.

---

### Remove a Package

```bash
sudo apt remove nginx
```

Removes a package from the system.

---

### Remove Unused Packages

```bash
sudo apt autoremove
```

Removes unused dependency packages.

---

## Commands Practiced

```bash
sudo apt update
sudo apt upgrade -y
sudo apt install nginx
apt search nginx
apt show nginx
sudo apt remove nginx
sudo apt autoremove
```

---

## What I Learned

- Updating package lists
- Upgrading installed packages
- Installing software using APT
- Searching for packages
- Viewing package information
- Removing packages