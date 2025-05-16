# Threadfin2 Setup Guide

Threadfin2 is responsible for managing local IPTV files and server in MediaCore.

## Storage Configuration

Threadfin2 is configured to use the following directory structure:

- **Config Path**: `/volume3/docker/threadfin/conf`
- **IPTV Path**: `/home/threadfin/conf/channeltest.m3u`
- **Guide Path**:  `/home/threadfin/conf/custom_epg.xml`

## Installation Detail

- **Docker Volume**: `/volume1/docker/threadfin2/config`
- **Docker Port**: 34445
- **Docker Network**: media_network

## Configuration Screenshots

### IPTV Settings
![Threadfin2 Settings](../images/threadfin2/settings.png)

## Integration with Other Services

- **Plex Integration**: How it connects to media servers

## Troubleshooting

- **Common Issue**: Stream buffering
  - **Solution**: Check network settings

