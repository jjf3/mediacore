# Radarr Setup Guide

Radarr is responsible for managing and automating movie downloads in MediaCore.

## Storage Configuration

Radarr is configured to use the following directory structure:

- **Download Path**: `/volume1/downloads/completed/movies`
- **Movies Library Path**: `/volume1/media/movies`

## Installation Details

- **Docker Volume**: `/volume1/docker/radarr/config`
- **Docker Port**: 8310
- **Docker Network**: media_network

## Configuration Screenshots

### Media Management Settings
![Radarr Media Management](../images/radarr/media-management.png)

## Integration with Other Services

### Jackett Integration
- **URL**: http://jackett:9117

### Transmission Integration
- **Host**: transmission
- **Port**: 9091

## Troubleshooting

- **Common Issue**: Permissions problems
  - **Solution**: Ensure proper permissions

