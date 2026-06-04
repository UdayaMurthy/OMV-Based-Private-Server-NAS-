# OMV-Based-Private-Server-NAS

A self-hosted home server built using OpenMediaVault and Debian.

## Features

* OpenMediaVault NAS
* Docker Services
* Tailscale Remote Access
* Jellyfin Media Streaming
* AdGuard Home DNS Filtering (In Progress)
* File Browser (Web File Manager)
* SMB Network Shares
* Automated Backup Planning
* Remote Administration

## Hardware

* **CPU:** Intel Core i3 Processor
* **RAM:** 2 GB (built from an older desktop system; upgrade planned in the future)
* **OS Drive:** 256 GB HDD
* **Storage Drive:** 1 TB HDD

## Network Architecture

```text
Internet
    │
Router
    │
Home Server
├── OpenMediaVault
├── Docker Engine
│   ├── Jellyfin
│   ├── File Browser
│   └── AdGuard Home
├── SMB Shares
└── Tailscale VPN
```

## Current/Completed Services

* ✅ OpenMediaVault
* ✅ Debian Installation
* ✅ Docker Environment
* ✅ Tailscale Remote Access
* ✅ Jellyfin Media Server
* ✅ File Browser
* ✅ SMB Network Shares
* 🚧 AdGuard Home (Configuration in Progress)

## In Progress

🟡 AdGuard Home

## Future Plans

* Homepage Dashboard
* Nextcloud
* Immich Photo Backup
* Monitoring with Grafana
* Automated Snapshots
* Prometheus
* Grafana

## Project Goals

This project repurposes an older desktop computer into a powerful home server for:

* Centralized file storage
* Secure remote access
* Media streaming
* Network-wide ad blocking
* Self-hosted applications
* Docker-based services

## Project Status

🟢 Active Development

The server is currently running OpenMediaVault, Tailscale, and Jellyfin successfully. AdGuard Home and additional self-hosted services are planned for future deployment.
