# Sonarr Setup Guide

Sonarr is responsible for managing and automating TV show downloads in MediaCore.

## Storage Configuration

Sonarr is configured to use the following directory structure:

- **Download Path**: `/volume2`
- **TV Library Path**: `
/volume2/Data/downloads
/volume2/Data/TV
/volume3/Data2/TV
/volume4/TV4`

## Installation Details

- **Docker Volume**: `/volume2`
- **Docker Port**: 8989
- **Docker Network**: Syno community

## Configuration Screenshots

### Media Management Settings
This was installed via Synology Package Center on Volume2.

## Integration with Other Services

### Jackett/Bazarr Integration
- Jacket: [http://your-nas-ip:9117](http://your-nas-ip:9117)
- Bazarr: [http://your-nas-ip:6767](http://your-nas-ip:6767)

### Transmission Integration
- **Host**: transmission
- **Port**: 9091

## Troubleshooting

- **Common Issue**: Permissions problems
  - **Solution**: Ensure proper permissions

