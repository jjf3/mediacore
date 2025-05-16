# Mediacore

MediaCore is a comprehensive, self-hosted media management solution that combines automated content acquisition with robust IPTV/DVR capabilities.
A self-hosted media server solution with automated TV/Movie downloads, Live TV DVR functionality, and comprehensive media management.

## Features

### Self-Contained Media System
- Local M3U and XML files
- Self-hosted EPG data server
- Integrated WebGrab+ for EPG updates
- Custom logo/data server

### Content Automation
- Automated TV show tracking (Sonarr)
- Automated movie downloads (Radarr)
- Configurable quality profiles
- Automatic subtitle management
- VPN integration for privacy

### Live TV & DVR
- Channel organization by category
- EPG data management
- DVR functionality for recording
- Threadfin and XTeve integration

### Reliability & Management
- Container health monitoring
- Automatic backups
- Permission management
- Detailed logging

## Quick Start

### Prerequisites
- Synology NAS or similar device
- Docker and Docker Compose installed
- Minimum 80 TB storage recommended (60TB main + 20TB backup)

### Access the services:
- Sonarr: http://your-nas-ip:8989
- Radarr: http://your-nas-ip:8310
- Jackett: http://your-nas-ip:9117
- Transmission: http://your-nas-ip:9091/web
- Threadfin2: http://your-nas-ip:34445 (local files and server)
- Threafin: http://your-nas-ip:34401/web/ (linked files and EPGBest)
- Plex: http://your-nas-ip:32400/
- Emby: http://your-nas-ip:8096/

## Configuration
See the Configuration Guide for detailed setup instructions.

## Maintenance
See the Maintenance Guide for routine maintenance tasks.

## Architecture
The system uses Docker containers orchestrated with Docker Compose. See the Architecture Document for details.

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
