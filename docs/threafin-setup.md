# Threafin Setup Guide

Threafin is responsible for managing linked IPTV files and EPGBest in MediaCore.

## Storage Configuration

Threafin is configured to use the following directory structure:

- **Config Path**: `/volume1/docker/threafin/config`
- **IPTV Path**: `/volume1/media/iptv`

## Installation Details

- **Docker Volume**: `/volume1/docker/threafin/config`
- **Docker Port**: 34401
- **Docker Network**: media_network

## Configuration Screenshots

### IPTV Settings
![Threafin Settings](../images/threafin/settings.png)

## Integration with Other Services

- **EPGBest Integration**: How it connects to EPG services
- **Plex Integration**: How it connects to media servers

## Troubleshooting

- **Common Issue**: EPG data missing
  - **Solution**: Check EPG source settings

