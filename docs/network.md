# Network Configuration

## Overview

This home server is connected to the local network through the home router and provides storage, media streaming, and remote access services.

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
├── Tailscale
└── AdGuard Home (Planned)
```

## Local Network

* Network Type: Private Home Network
* IP Address Range: 192.168.X.X
* Connection Method: Ethernet

### Server Local Access

OpenMediaVault can be accessed from devices connected to the local network using:

```text
http://192.168.X.X/24
```

## Remote Access

Remote access is provided through Tailscale.

### Tailscale Benefits Are as

* Secure encrypted connections
* No port forwarding required
* Access from laptops, desktops, and mobile devices
* Private network communication between authorized devices

The server can be accessed remotely through Tailscale using SSH:

ssh <username>@<tailscale-device>

Example:

ssh user@homeserver

### Remote Management

The server can be accessed remotely using:

```bash
ssh openmediavault@192.168.X.X
```

or through the Tailscale-assigned device name.

## Services

| Service        | Purpose         | Access Method             |
| -------------- | --------------- | ------------------------- |
| OpenMediaVault | NAS Management  | Local Network / Tailscale |
| Jellyfin       | Media Streaming | Local Network / Tailscale |
| Tailscale      | Remote Access   | Internet                  |
| AdGuard Home   | DNS Filtering   | Planned                   |

## Future Improvements

* Configure AdGuard Home as the primary DNS server
* Implement monitoring and alerting (PROMETHEUS & GRAFANA)
* Add dashboard for service management
* Expand Docker-based services
