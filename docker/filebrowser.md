# File Browser

## Overview

File Browser is a web-based file management application deployed using Docker on the OpenMediaVault server.

## Purpose

* Access files through a web browser
* Upload and download files remotely
* Create and manage folders
* Organize media and server data
* Simplify file management without SSH access

## Deployment

The service is deployed using Docker Compose through OpenMediaVault.

## Access Method

The File Browser web interface can be accessed from devices connected through the local network or remotely using Tailscale.

## Storage

File Browser is configured to access the server storage directories used by OpenMediaVault.

## Future Improvements

* HTTPS support
* User-specific permissions
* Homepage dashboard integration
* Backup configuration

