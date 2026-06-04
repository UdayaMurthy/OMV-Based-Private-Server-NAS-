# Jellyfin Media Server

## Overview

Jellyfin is the primary self-hosted media streaming service running on this server.

The service is deployed as a Docker container using the OpenMediaVault Compose Plugin.

## Purpose

Jellyfin provides:

* Movie streaming
* TV show streaming
* Music streaming
* Multi-device media access
* Remote media access through Tailscale

## Deployment

### Platform

* Docker Container
* Managed through OpenMediaVault Compose Plugin

### Access

Local Access:

```text
http://<SERVER_IP>:8096
```

Remote Access:

```text
Through Tailscale network
```

## Media Storage

Media is stored on the dedicated data drive.

Library categories include:

* Movies
* TV Shows
* Music

## Container Configuration

### Volumes

```text
/config
/media
```

### Network

```text
Port: 8096
```

## Features Enabled

* Metadata retrieval
* Automatic library scanning
* Multi-user support
* Web-based administration

## Backup Strategy

Important items to back up:

* Jellyfin configuration
* Metadata database
* Docker Compose configuration
* Media library structure

Media files are stored separately on the data drive.

## Recovery Procedure

1. Deploy Jellyfin container.
2. Restore configuration files.
3. Connect media directories.
4. Verify library detection.
5. Rescan media content.

## Future Improvements

* Hardware acceleration
* Expanded media libraries
* Additional user profiles
* Enhanced remote streaming support

