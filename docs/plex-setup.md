# Sonarr Setup Guide

Plex is responsible for managing and playing media content mostly TV shows and some movies. 

## Storage Configuration

Plex is configured to use the following directory structure:

- **Download Path**: `/volume2`
- **TV Library Path**: `
/volume2/Data/downloads
/volume2/Data/TV
/volume3/Data2/TV
/volume4/TV4`

## Installation Details

- **Docker Volume**: `/volume2`
- **Docker Port**: 32400
- **Docker Network**: Syno community

## Configuration Screenshots

### Media Management Settings
This was installed via Synology Package Center on Volume2.

## Integration with Other Services

### Arr Integrations
- Jacket: [http://your-nas-ip:9117](http://your-nas-ip:9117)
- Bazarr: [http://your-nas-ip:6767](http://your-nas-ip:6767)
- Sonarr: [http://your-nas-ip:8989](http://your-nas-ip:8989)
- Radarr: [http://your-nas-ip:8310](http://your-nas-ip:8310)
- Transmission: [http://your-nas-ip:9091/web](http://your-nas-ip:9091/web)
- Nginx: [http://your-nas-ip:8085/](http://your-nas-ip:8085)

