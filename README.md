# Plex Media Server Homelab Project

This project documents the process of building a personal Plex Media Server using Proxmox virtualization.

The goal of this project is to host movies and TV shows that can be accessed remotely from any device.

---

## Project Overview

This setup uses a Windows 11 virtual machine running inside Proxmox to host Plex Media Server.

Features:

- Virtualized media server
- Remote streaming
- Custom media libraries
- VPN support
- Router port forwarding

---

## Hardware Used

Host Machine: Dell Latitude 7450  
CPU: Intel i5-5300U  
RAM: 32GB  
Storage: 100GB SSD  
Graphics: Intel HD Graphics 5500

---

## Software Stack

- Proxmox VE
- Windows 11 VM
- Plex Media Server
- VirtIO Drivers
- Private Internet Access VPN

---

## Architecture

Laptop (Proxmox Host)
      │
      ▼
Windows 11 Virtual Machine
      │
      ▼
Plex Media Server
      │
      ▼
Remote Streaming Devices

---

## Installation Guide

Detailed setup documentation:

- [Installing Proxmox](docs/proxmox-install.md)
- [Creating the Windows VM](docs/vm-creation.md)
- [Installing Plex](docs/plex-install.md)
- [Router Port Forwarding](docs/router-config.md)

---

## Media Library Structure

```
Plex/
 ├── Movies/
 └── TV Shows/
```

---

## Remote Access

Remote streaming is enabled using:

- Router Port Forwarding
- Plex Remote Access Settings

---

## Testing

To test the server:

1. Log into Plex from another device.
2. Navigate to Movies or TV Shows.
3. Confirm media streams correctly.

---

## Future Improvements

- Migrate Plex to Linux container
- Add automated media downloads
- Implement NAS storage
- Add monitoring (Grafana/Prometheus)

---

## Skills Demonstrated

- Virtualization
- Server deployment
- Network configuration
- Port forwarding
- Media server management
