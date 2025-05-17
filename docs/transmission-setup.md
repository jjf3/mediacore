# Transmission Setup Guide

Transmission is responsible for managing torrent downloads in MediaCore.

## Storage Configuration

Transmission is configured to use the following directory structure:

- **Download Path**: `/volume1/downloads`
- **Completed Path**: `/volume1/downloads/completed`

## Installation Details

- **Docker Volume**: `/volume2/`
- **Docker Port**: 9091
- **Docker Network**: media_network

## Configuration Screenshots

### Download Settings
This was installed via Synology Package Center on Volume2.

## Integration with Other Services

For a better torrent management experience I highly recommend setting up Transgui: https://github.com/transmission-remote-gui/transgui

- **Sonarr/Radarr Integration**: How it connects

