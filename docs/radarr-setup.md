# Radarr Setup Guide

Radarr is responsible for managing and automating movie downloads in MediaCore.

## Storage Configuration

Radarr is configured to use the following directory structure:

- **Download Path**: `/volume3`
- **Movies Library Path**: `/volume4/Movies4`

## Installation Details

- **Docker Volume**: `/volume3`
- **Docker Port**: 8310
- **Docker Network**: Syno community

## Configuration Screenshots

### Media Management Settings
This was installed via Synology Package Center on Volume3.

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

