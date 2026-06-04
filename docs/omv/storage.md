# Storage Configuration

## Overview

The home server uses separate drives for the operating system and media storage. This separation improves manageability and simplifies future upgrades.

---

## Drives

### OS Drive

* Size: 256 GB HDD
* Purpose: Debian Operating System and OpenMediaVault
* Status: Active

### Media Drive

* Size: 1 TB HDD
* Purpose: Media Storage and Shared Data
* Status: Active

---

## Shared Folders

### Media

Purpose:

* Stores movies, TV shows, and music
* Used by Jellyfin for media streaming

Access:

* OpenMediaVault
* Jellyfin
* File Browser
* SMB Shares

### Downloads

Purpose:

* Temporary storage for downloaded files
* Media organization and file transfers

Access:

* OpenMediaVault
* File Browser
* SMB Shares

### Backups

Purpose:

* Configuration backups
* Recovery files
* Future automated backup storage

Access:

* Administrator Only

---

## Service Storage Usage

| Service        | Storage Purpose             |
| -------------- | --------------------------- |
| OpenMediaVault | System Management           |
| Jellyfin       | Media Library               |
| File Browser   | File Access and Management  |
| Docker         | Container Configuration     |
| AdGuard Home   | DNS Configuration (Planned) |

---

## Current Storage Layout

```text
256 GB HDD
└── Debian
    └── OpenMediaVault

1 TB HDD
├── Media
├── Downloads
└── Backups
```

---

## Future Improvements

* Upgrade system memory
* Implement automated backups
* Configure snapshot-based recovery
* Expand storage capacity as media collection grows

---

## Recovery Notes

In the event of a server rebuild:

1. Install Debian.
2. Install OpenMediaVault.
3. Reconnect the 1 TB media drive.
4. Recreate shared folders if required.
5. Restore Docker Compose files.
6. Restore service configurations.
7. Verify Jellyfin, File Browser, and network access.

This document should be updated whenever storage devices or shared folders are modified.
