# Mediacore

MediaCore is a comprehensive, self-hosted media management solution that combines automated content acquisition with robust IPTV/DVR capabilities.
A self-hosted media server solution with automated TV/Movie downloads, Live TV DVR functionality, and comprehensive media management.

## Features

### Self-Contained Media System
- Local M3U and XML files - Created and In Progress of Configuring
- Self-hosted EPG data server - Created and In Progress of Configuring
- Integrated WebGrab+ for EPG updates - To do 
- Custom logo/data server - to do

### Content Automation
- Automated TV show tracking (Sonarr) - Complete
- Automated movie downloads (Radarr) - Complete
- Configurable quality profiles - Complete
- Automatic subtitle management - Complete
  

### Live TV & DVR 
- Channel organization by category - In Progress
- EPG data management - In Progress
- DVR functionality for recording - In Progress
- Threadfin and XTeve integration - In Progress

### Reliability & Management - This is done by the Synology NAS
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

Below you'll find detailed setup guides for each component of the MediaCore system:

| Component | Description | Status | Documentation |
|-----------|-------------|--------|---------------|
| Sonarr | TV show management and automation | Complete | [Setup Guide](./docs/sonarr-setup.md) |
| Radarr | Movie management and automation | Complete | [Setup Guide](./docs/radarr-setup.md) |
| Jackett | Torrent indexer proxy | Complete | [Setup Guide](./docs/jackett-setup.md) |
| Plex | Media server and playback | Complete | [Setup Guide](./docs/plex-setup.md) |
| Emby | Media server and playback | Complete | [Setup Guide](./docs/emby-setup.md) |
| Original Threadfin | M3U/EPG proxy | Conmplete | [Setup Guide](./docs/threadfin-setup.md) |
| Second Threadfin | M3U/EPG proxy | In Progress | [Setup Guide](./docs/threadfin2-setup.md) |
| Transmission | Download client | Complete | [Setup Guide](./docs/transmission-setup.md) |
| WebGrab+ | EPG data acquisition | To Do | [Setup Guide](./docs/webgrab-setup.md) |

## Maintenance
See the Maintenance Guide for routine maintenance tasks.

## Architecture
The system uses Docker containers orchestrated with Docker Compose. See the Architecture Document for details.

## Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
