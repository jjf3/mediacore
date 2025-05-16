# Sonarr Setup Guide

Sonarr is responsible for managing and automating TV show downloads in MediaCore.

## Storage Configuration

Sonarr is configured to use the following directory structure:

- **Download Path**: `/volume1/downloads/completed/tv`
- **TV Library Path**: `/volume1/media/tv`

## Installation Details

- **Docker Volume**: `/volume1/docker/sonarr/config`
- **Docker Port**: 8989
- **Docker Network**: media_network

## Configuration Screenshots

### Media Management Settings
![Sonarr Media Management](../images/sonarr/media-management.png)

## Integration with Other Services

### Jackett Integration
- **URL**: http://jackett:9117

### Transmission Integration
- **Host**: transmission
- **Port**: 9091

## Troubleshooting

- **Common Issue**: Permissions problems
  - **Solution**: Ensure proper permissions

