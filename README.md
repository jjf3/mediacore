# MediaCore

MediaCore is a comprehensive, self-hosted media management solution that combines automated content acquisition with robust IPTV/DVR capabilities.

![Project Status](https://img.shields.io/badge/status-beta-yellow)
![License](https://img.shields.io/badge/license-MIT-blue)

## Overview

MediaCore integrates multiple open-source services to create a complete media server solution featuring:
- Automated TV shows and movies downloads
- Live TV with DVR functionality
- EPG (Electronic Program Guide) management
- Multiple media server options for playback

## Features

| Feature | Description | Status |
|---------|-------------|--------|
| | <div align="center">**Self-Contained Media System**</div> | |
| Local M3U and XML files | Core playlist and metadata files | 🟡 In Progress |
| Self-hosted EPG data server | Local EPG management | 🟡 In Progress |
| Integrated WebGrab+ | EPG updates automation | 🔴 To Do |
| Custom logo/data server | Artwork and metadata management | 🔴 To Do |
| **Content Automation** | | |
| Sonarr integration | TV show tracking and downloads | ✅ Complete |
| Radarr integration | Movie downloads | ✅ Complete |
| Quality profiles | Configurable media quality | ✅ Complete |
| Subtitle management | Automatic subtitle downloads | ✅ Complete |
| | <div align="center">**Live TV & DVR**</div> | |
| Channel categorization | Organization by content type | 🟡 In Progress |
| EPG data management | Program guide handling | 🟡 In Progress |
| DVR functionality | Live TV recording | 🟡 In Progress |
| Threadfin and XTeve | IPTV proxy integration | 🟡 In Progress |
| **Reliability & Management** | Provided by Synology NAS | ✅ Complete |

## Installation

### Prerequisites
- Synology NAS or similar device
- Docker and Docker Compose installed
- Minimum 80 TB storage recommended (60TB main + 20TB backup)


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

## Architecture
The system uses Docker containers orchestrated with Docker Compose. See the Architecture Document [Setup Guide](./docs/architecture.md) for details.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
