# Users and Permissions

## Overview

User accounts and permissions are managed through OpenMediaVault to control access to shared folders, services, and remote administration features.

---

## User Types

### Administrator

Purpose:

* Server management
* OpenMediaVault administration
* Docker service management
* System maintenance and updates

Permissions:

* Full access to server resources
* Full access to shared folders
* Service configuration and management

---

### Standard Users

Purpose:

* Access shared files and media
* Use network services

Permissions:

* Access only to authorized shared folders
* No administrative privileges

---

## Service Access

| Service        | Access Type        |
| -------------- | ------------------ |
| OpenMediaVault | Administrator      |
| Docker         | Administrator      |
| Jellyfin       | Authorized Users   |
| File Browser   | Authorized Users   |
| SMB Shares     | Authorized Users   |
| Tailscale      | Authorized Devices |

---

## Shared Folder Permissions

### Media

Access:

* Read/Write: Administrator
* Read Access: Authorized Users

---

### Downloads

Access:

* Read/Write: Administrator
* Read/Write: Authorized Users

---

### Backups

Access:

* Administrator Only

---

## Remote Access Security

Remote access is provided through Tailscale.

Security measures:

* Encrypted communication
* Device-based authentication
* No public port forwarding
* Access limited to authorized devices

---

## Permission Management

Permissions are managed through the OpenMediaVault web interface.

Changes should be documented whenever:

* New users are added
* Shared folder permissions are modified
* New services are deployed
* Remote access policies are changed

---

## Security Notes

* Administrative accounts should use strong passwords.
* Only authorized users should have access to shared folders.
* Remote administration should be restricted to trusted devices.
* Sensitive credentials should never be stored in this repository.

