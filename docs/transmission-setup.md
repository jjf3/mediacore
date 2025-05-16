# Transmission Setup Guide

Transmission is responsible for managing torrent downloads in MediaCore.

## Storage Configuration

Transmission is configured to use the following directory structure:

- **Download Path**: `/volume1/downloads`
- **Completed Path**: `/volume1/downloads/completed`

## Installation Details

- **Docker Volume**: `/volume1/docker/transmission/config`
- **Docker Port**: 9091
- **Docker Network**: media_network

## Configuration Screenshots

### Download Settings
![Transmission Settings](../images/transmission/settings.png)

## Integration with Other Services

- **VPN Configuration**: Details of VPN setup
- **Sonarr/Radarr Integration**: How it connects

## Troubleshooting

- **Common Issue**: VPN connectivity
  - **Solution**: Check VPN status

