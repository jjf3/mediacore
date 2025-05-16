# Jackett Setup Guide

Jackett is responsible for managing indexer connections in MediaCore.

## Storage Configuration

Jackett is configured to use the following directory structure:

- **Config Path**: `/volume1/docker/jackett/config`

## Installation Details

- **Docker Volume**: `/volume1/docker/jackett/config`
- **Docker Port**: 9117
- **Docker Network**: media_network

## Configuration Screenshots

### Indexer Settings
![Jackett Indexers](../images/jackett/indexers.png)

## Integration with Other Services

- **Sonarr API Key**: Configure in Sonarr
- **Radarr API Key**: Configure in Radarr

## Troubleshooting

- **Common Issue**: Indexer connectivity
  - **Solution**: Check indexer status

