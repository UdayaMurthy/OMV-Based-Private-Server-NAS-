# Network Configuration

## Overview

This home server is connected to the local network through the home router and provides storage, media streaming, and secure remote access services.

---

## Network Architecture

```text
Internet
    │
    ▼
Router
    │
    ▼
Home Server
├── OpenMediaVault
├── Jellyfin
├── File Browser
├── Tailscale
└── AdGuard Home (Planned)
```

---

## Local Network

| Setting           | Value                |
| ----------------- | -------------------- |
| Network Type      | Private Home Network |
| IP Address Range  | 192.168.x.x          |
| Connection Method | Ethernet             |

---

## Local Access

OpenMediaVault and other services can be accessed from devices connected to the local network.

### Example

```text
http://192.168.x.x
```

---

## Remote Access

Remote access is provided through Tailscale.

### Benefits

* Secure encrypted connections
* No port forwarding required
* Access from laptops, desktops, and mobile devices
* Private communication between authorized devices
* Simplified remote administration

---

## SSH Access

The server can be accessed remotely using SSH through the Tailscale network.

### Example

```bash
ssh <username>@<tailscale-device>
```

Example:

```bash
ssh user@homeserver
```

---

## Remote Management

Services can be managed remotely through:

* SSH
* OpenMediaVault Web Interface
* Jellyfin Web Interface
* File Browser Web Interface

Access is available through the local network or the Tailscale network.

---

## Services

| Service        | Purpose         | Access Method             |
| -------------- | --------------- | ------------------------- |
| OpenMediaVault | NAS Management  | Local Network / Tailscale |
| Jellyfin       | Media Streaming | Local Network / Tailscale |
| File Browser   | File Management | Local Network / Tailscale |
| Tailscale      | Remote Access   | Internet                  |
| AdGuard Home   | DNS Filtering   | Planned                   |

---

## Future Improvements

* Configure AdGuard Home as the primary DNS server
* Implement monitoring and alerting using Grafana and Prometheus
* Deploy a Homepage dashboard for centralized service management
* Expand Docker-based services
* Implement automated backup and recovery workflows

---

## Security Notes

* No services are exposed directly to the internet.
* Remote access is secured through Tailscale.
* Administrative access is restricted to authorized devices.
* SSH is used for remote server management.

```
```
