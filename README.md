# mediacore
MediaCore is a comprehensive, self-hosted media management solution that combines automated content acquisition with robust IPTV/DVR capabilities.


A self-hosted media server solution with automated TV/Movie downloads, Live TV DVR functionality, and comprehensive media management.
Features

Self-Contained Media System

Local M3U and XML files
Self-hosted EPG data server
Integrated WebGrab+ for EPG updates
Custom logo/data server


Content Automation

Automated TV show tracking (Sonarr)
Automated movie downloads (Radarr)
Configurable quality profiles
Automatic subtitle management
VPN integration for privacy


Live TV & DVR

Channel organization by category
EPG data management
DVR functionality for recording
Threadfin and XTeve integration


Reliability & Management

Container health monitoring
Automatic backups
Permission management
Detailed logging



Quick Start
Prerequisites

Synology NAS or similar device
Docker and Docker Compose installed
Minimum 34TB storage recommended (20TB main + 14TB backup)

Installation

Clone this repository:

bashgit clone https://github.com/yourusername/mediaserver.git
cd mediaserver

Run the setup script:

bashsudo ./setup.sh

Start the services:

bashdocker-compose up -d

Access the services:

Sonarr: http://your-nas-ip:8989
Radarr: http://your-nas-ip:8310
Jackett: http://your-nas-ip:9117
Transmission: http://your-nas-ip:9091/web
Threadfin: http://your-nas-ip:34401
XTeve: http://your-nas-ip:34400/web/



Configuration
See the Configuration Guide for detailed setup instructions.
Maintenance
See the Maintenance Guide for routine maintenance tasks.
Architecture
The system uses Docker containers orchestrated with Docker Compose. See the Architecture Document for details.
Contributing
Contributions are welcome! Please feel free to submit a Pull Request.
License
This project is licensed under the MIT License - see the LICENSE file for details.
