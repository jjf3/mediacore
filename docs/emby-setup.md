# Emby Setup Guide

Emby is responsible for managing and playing live TV.  

## Storage Configuration

Plex is configured to use the following directory structure:

- **Download Path**: `/volume2`


## Installation Details

- **Docker Volume**: `/volume2`
- **Docker Port**: 8096
- **Docker Network**: Syno community

## Configuration Screenshots

### Media Management Settings
This was installed via Synology Package Center on Volume2.

## Integration with Other Services
For live TV setup just point your m3u and guide sources to the link provided by the load balancer which can be found on port 8085/playlist.m3u and 8085/epg.xml

