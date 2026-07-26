# Networking

## Overview

Networking is used to connect computers and servers so they can communicate with each other. Linux provides many commands to check network connectivity, IP addresses, DNS, and open ports.

---

## Common Commands

### Check IP Address

```bash
ip a
```

Displays the IP address and network interfaces of the system.

---

### Check Hostname

```bash
hostname
```

Displays the system hostname.

---

### Test Network Connectivity

```bash
ping google.com
```

Checks if the system can communicate with another host.

Press **Ctrl + C** to stop the ping command.

---

### Display Active Network Connections

```bash
ss -tuln
```

Shows listening TCP and UDP ports.

---

### Check DNS Information

```bash
nslookup google.com
```

Looks up the IP address of a domain name.

> If `nslookup` is not installed:

```bash
sudo apt install dnsutils
```

---

### Download a File

```bash
wget https://example.com
```

Downloads a file from the internet.

---

### Fetch Data from a Website

```bash
curl https://example.com
```

Displays the webpage content in the terminal.

---

## Commands Practiced

```bash
ip a
hostname
ping google.com
ss -tuln
nslookup google.com
wget https://example.com
curl https://example.com
```

---

## What I Learned

- How to check the IP address
- How to check the hostname
- How to test network connectivity
- How to check listening ports
- How to perform a DNS lookup
- How to download files using wget
- How to fetch website content using curl

---

## Conclusion

In this lab, I learned basic Linux networking commands. These commands are useful for checking connectivity, troubleshooting network issues, and gathering network information.
