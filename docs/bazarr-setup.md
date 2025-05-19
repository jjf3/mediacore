# Bazarr Setup Guide

Bazarr is responsible for managing and automating subtitle downloads in MediaCore.

## Storage Configuration

Sonarr is configured to use the following directory structure:

- **Download Path**: `/volume3`

## Installation Details

- **Docker Volume**: `/volume3`
- **Docker Port**: 6767
- **Docker Network**: Syno community

## Configuration Screenshots

### Media Management Settings
This was installed via Synology Package Center on Volume2.

## Other Tools
You can use Pasta to quckly change default subtitles in all your movie/tv shows. My Pasta instance was installed using dokcer and can be found on port 8087

## Troubleshooting

- **Common Issue**: Permissions problems
  - **Solution**: Ensure proper permissions

