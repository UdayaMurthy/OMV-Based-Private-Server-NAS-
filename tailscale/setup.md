# Tailscale Setup

## Overview

Tailscale is used to provide secure remote access to the home server without requiring port forwarding or exposing services directly to the internet.

The server is connected to a private Tailnet, allowing authorized devices to securely access services from anywhere.

## Purpose

Tailscale provides:

* Secure remote administration
* Encrypted device-to-device communication
* Access to services outside the local network
* Simplified VPN connectivity
* SSH access to the server

## Deployment

### Platform

* Installed on the server
* Connected to a private Tailnet
* Enabled for remote management

## Access Methods

### SSH Access

The server can be accessed remotely using:

```bash
ssh <username>@<tailscale-device>
```

### Service Access

The following services can be accessed through the Tailscale network:

* OpenMediaVault
* Jellyfin
* Docker-hosted services
* Future self-hosted applications

## Security Benefits

* No port forwarding required
* End-to-end encrypted connections
* Device-based authentication
* Private network access
* Reduced attack surface

## Connected Devices

Authorized devices may include:

* Home Server
* Laptop
* Desktop
* Mobile Devices

## Maintenance

### Verification

Verify connectivity by:

1. Checking Tailscale status
2. Confirming device visibility within the Tailnet
3. Testing SSH connectivity
4. Verifying access to hosted services

## Recovery Procedure

If remote access is lost:

1. Verify internet connectivity.
2. Check Tailscale service status.
3. Re-authenticate the server to the Tailnet if required.
4. Confirm device authorization.
5. Test SSH access again.

## Future Improvements

* Additional device enrollment
* Enhanced access controls
* Service-specific access policies
* Monitoring and alerting integration

## Notes

Tailscale serves as the primary remote access solution for this home server project.
