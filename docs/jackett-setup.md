# Jackett Setup Guide

Jackett is responsible for managing indexer connections in MediaCore.

## Storage Configuration

Jackett is configured to use the following directory structure:

- **Config Path**: `/volume2/`

## Installation Details

- **Docker Volume**: `/volume2/`
- **Docker Port**: 9117
- **Docker Network**: syno community

## Configuration Screenshots

### Indexer Settings
This was installed via Synology Package Center on Volume2.

## Integration with Other Services

- **Sonarr API Key**: Configure in Sonarr
- **Radarr API Key**: Configure in Radarr

## Troubleshooting

- **Common Issue**: Indexer connectivity
  - **Solution**: Check indexer status

