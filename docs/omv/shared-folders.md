# Shared Folders

## Overview

Shared folders are used to organize and provide access to data stored on the home server.

These folders are accessible through OpenMediaVault services, SMB network shares, Docker containers, and File Browser where applicable.

---

## Media

### Purpose

Stores movies, TV shows, music, and other media content.

### Used By

* Jellyfin
* File Browser
* SMB Shares

### Access

* Local Network
* Tailscale Remote Access

---

## Downloads

### Purpose

Temporary storage for downloaded files and media organization.

### Used By

* File Browser
* SMB Shares

### Access

* Local Network
* Tailscale Remote Access

---

## Backups

### Purpose

Stores configuration backups and recovery files.

### Used By

* System Administrator

### Access

* Administrator Only

---

## Permissions

Permissions are managed through OpenMediaVault.

Access is granted only to authorized users and services.

---

## Notes

Shared folders should be backed up regularly and reviewed whenever new services are deployed.

This document should be updated whenever shared folders are added, removed, or modified.
