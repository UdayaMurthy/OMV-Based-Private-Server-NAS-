# Docker Setup

## Overview

Docker is used to host and manage self-hosted services on the server.

The Docker environment is managed through the OpenMediaVault Compose Plugin.

## Purpose

Docker provides:

* Service isolation
* Easy deployment
* Simplified updates
* Configuration portability

## Docker Management

Docker containers are managed through:

* OpenMediaVault Web Interface
* Compose Plugin
* Docker Compose YAML files

## Current Containers

| Service      | Status           | Purpose         |
| ------------ | ---------------- | --------------- |
| Jellyfin     | Active           | Media Streaming |
| AdGuard Home | Planned          | DNS Filtering   |

## Deployment Method

Services are deployed using Docker Compose YAML files.

Typical workflow:

1. Create a Compose stack.
2. Configure service settings.
3. Deploy stack through OMV.
4. Verify container health.
5. Monitor service logs.

## Container Updates

General update procedure:

1. Pull updated container images.
2. Redeploy stack.
3. Verify service functionality.
4. Check logs for errors.

## Backup Strategy

Important items to back up:

* Compose YAML files
* Service configuration directories
* Application data volumes

## Future Services

Planned Docker deployments:

* Homepage Dashboard
* Immich
* Grafana
* Additional self-hosted applications
