# OMV-Based-Private-Server-NAS

A self-hosted home server built using OpenMediaVault and Debian.

## Features

* OpenMediaVault NAS
* Tailscale Remote Access
* Jellyfin Media Streaming
* AdGuard Home DNS Filtering
* SMB Network Shares
* Automated Backups
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
    ▼
Router
    │
    ▼
Home Server
├── OpenMediaVault
├── Jellyfin
├── AdGuard Home
├── Tailscale
└── Docker Containers
```

## Current Services

* ✅ OpenMediaVault
* ✅ Tailscale
* ✅ Jellyfin
* 🚧 AdGuard Home (Configuration in Progress)

## Future Plans

* Homepage Dashboard
* Nextcloud
* Immich Photo Backup
* Monitoring with Grafana
* Automated Snapshots

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
