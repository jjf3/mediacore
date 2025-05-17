# Transmission Setup Guide

Transmission is responsible for managing torrent downloads in MediaCore.

## Storage Configuration

Transmission is configured to use the following directory structure:

- **Download Path**: `/volume3/Data2/TV` (or whatever your largest directory is. 
- **Incomplete Path**: `/volume3/Data2/TV/incomplete`
- **Optional Path(s)** volume `/volume4/TV4, /volume2/Data/TV` or wherever you have free space.

## Installation Details

- **Docker Volume**: `/volume2/`
- **Docker Port**: 9091
- **Docker Network**: syno community

## Configuration Screenshots

### Download Settings
This was installed via Synology Package Center on Volume2.

## Integration with Other Services

For a better torrent management experience I highly recommend setting up Transgui: https://github.com/transmission-remote-gui/transgui

- **Sonarr/Radarr Integration**: How it connects

