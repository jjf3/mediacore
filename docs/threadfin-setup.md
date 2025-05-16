# Threafin Setup Guide

This is my original Threafin which is responsible for managing linked IPTV files and EPGBest in MediaCore.

# Threadfin Setup Documentation

## Container Configuration

The Threadfin container is configured as follows:

- **Container Name**: fyb3roptik-threadfin-1
- **Container ID**: dd0fa76ce2236f496d3826e1fcbd9880c576f2a540920225c13a8981ec43afd3 (this is due to change)
- **Image**: fyb3roptik/threadfin:latest
- **Port Mapping**: 34400/tcp → 34401

## File System Layout

### Docker Container

The Threadfin application is installed inside the Docker container with the following directory structure:

- **Home Directory**: `/home/threadfin`
  - **Binary Files**: `/home/threadfin/bin`
  - **Configuration**: `/home/threadfin/conf`
  - **Cache**: `/home/threadfin/cache`
  - **Temporary Files**: `/tmp/threadfin`

### Volume Mounts

The container has a volume mount configured:
- **Source**: `/volume3/Data2`
- **Destination**: `/Docker`
- **Mode**: `rw` (read-write)

However, the Docker directory appears to be empty, suggesting that the application may not be using this volume for persistent storage as expected.

## Accessing Configuration Files

To access the Threadfin configuration files:

1. SSH into your Synology NAS
2. Execute a shell inside the container:
   ```bash
   docker exec -it dd0fa76ce2236f496d3826e1fcbd9880c576f2a540920225c13a8981ec43afd3 (yours is different) /bin/sh
   ```
3. Navigate to the configuration directory:
   ```bash
   ls -la /home/threadfin/conf
   ```

## Important Environment Variables

The container has the following environment variables set:

- **PATH**: `/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/home/threadfin/bin`
- **THREADFIN_BIN**: `/home/threadfin/bin`
- **THREADFIN_CONF**: `/home/threadfin/conf`
- **THREADFIN_HOME**: `/home/threadfin`
- **THREADFIN_TEMP**: `/tmp/threadfin`
- **THREADFIN_CACHE**: `/home/threadfin/cache`
- **THREADFIN_UID**: `31337`
- **THREADFIN_GID**: `31337`
- **THREADFIN_USER**: `threadfin`

## Backing Up Configuration

=## Notes

- The configuration files are stored within the container at `/home/threadfin/conf`
- For future container recreations, you may need to manually back up and restore the configuration from within the container
