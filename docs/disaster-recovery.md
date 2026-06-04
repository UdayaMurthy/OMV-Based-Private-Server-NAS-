# Disaster Recovery Guide

## Purpose

This document describes the steps required to recover and rebuild the home server in case of operating system failure, drive failure, or accidental misconfiguration.

## Current Hardware

* CPU: Intel Core i3
* RAM: 2 GB
* OS Drive: 256 GB HDD
* Data Drive: 1 TB HDD

## Recovery Scenario 1: Operating System Failure

### Symptoms

* Server fails to boot
* OpenMediaVault becomes inaccessible
* System corruption

### Recovery Steps

1. Download the latest OpenMediaVault installation image.
2. Reinstall OpenMediaVault on the OS drive.
3. Configure network settings.
4. Reinstall Docker and Docker Compose.
5. Restore service configurations.
6. Reconnect data drives.
7. Verify SMB shares and permissions.

## Recovery Scenario 2: Docker Service Failure

### Recovery Steps

1. Verify Docker service status.
2. Restart Docker.
3. Restore Docker Compose files.
4. Redeploy containers.
5. Verify container functionality.

## Recovery Scenario 3: Jellyfin Failure

### Recovery Steps

1. Recreate the Jellyfin container.
2. Restore configuration backup.
3. Verify media library paths.
4. Rescan media libraries.

## Recovery Scenario 4: Tailscale Failure

### Recovery Steps

1. Reinstall Tailscale.
2. Re-authenticate with the Tailnet.
3. Verify remote connectivity.
4. Test SSH access.

## Recovery Scenario 5: Data Drive Failure

### Recovery Steps

1. Replace failed drive.
2. Restore data from backup.
3. Verify file permissions.
4. Reconnect services to restored data.

## Important Notes

* Keep Docker Compose files backed up.
* Keep OMV configuration backups.
* Maintain copies of important documentation.
* Test backups periodically.

## Future Improvements

* Automated backups
* Scheduled configuration exports
* Off-site backup strategy
* Recovery testing procedures

