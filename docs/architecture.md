# Enhanced Self-Hosted Media Server Architecture

## Project Overview
This repository manages a self-hosted media server ecosystem with automated TV/Movie downloads, Live TV DVR functionality, and comprehensive media management. The system uses Docker containers for services and implements Infrastructure as Code (IaC) for reproducibility and maintenance.

## Architecture Diagram
```
┌───────────────────────────────────────────────────────────────────┐
│                      Synology NAS (80TB)                          │
│                                                                   │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌──────────┐  │
│  │   Docker    │  │  File Mgmt  │  │    Backup   │  │  Security│  │
│  │ Containers  │  │   System    │  │   System    │  │  System  │  │
│  └─────────────┘  └─────────────┘  └─────────────┘  └──────────┘  │
│         │                │                │               │       │
│         ▼                ▼                ▼               ▼       │
│  ┌─────────────────────────────────────────────────────────────┐  │
│  │                   Docker Network                            │  │
│  │                                                             │  │
│  │  ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐            │  │
│  │  │ Sonarr  │ │ Radarr  │ │ Jackett │ │ Trans-  │            │  │
│  │  │ (8989)  │ │ (8310)  │ │ (9117)  │ │ mission │            │  │
│  │  └─────────┘ └─────────┘ └─────────┘ │ (9091)  │            │  │
│  │       │           │           │      └─────────┘            │  │
│  │       │           │           │           │                 │  │
│  │       ▼           ▼           ▼           ▼                 │  │
│  │  ┌────────────────────────────────────────────────────┐     │  │
│  │  │                  Media Management                  │     │  │
│  │  └────────────────────────────────────────────────────┘     │  │
│  │                                                             │  │
│  │  ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌───────┐  │  │
│  │  │Threadfin│ │ 2thread │ │ │WebGrab│ │EPG Data │ │Local  │  │  │
│  │  │ (34401) │ │ (34445) │ │Plus     │ │Server   │ │M3U/XML│  │  │
│  │  └─────────┘ └─────────┘ └─────────┘ └─────────┘ └───────┘  │  │
│  │       │           │           │           │          │      │  │
│  │       ▼           ▼           ▼           ▼          ▼      │  │
│  │  ┌────────────────────────────────────────────────────┐     │  │
│  │  │                   IPTV/DVR System                  │     │  │
│  │  └────────────────────────────────────────────────────┘     │  │
│  │                                                             │  │
│  │  ┌─────────┐ ┌─────────┐                                    │  │
│  │  │  Plex   │ │  Emby   │                                    │  │
│  │  │ Media   │ │ Media   │                                    │  │
│  │  │ Server  │ │ Server  │                                    │  │
│  │  └─────────┘ └─────────┘                                    │  │
│  └─────────────────────────────────────────────────────────────┘  │
└───────────────────────────────────────────────────────────────────┘
```

## Key Improvements
1. **Self-Contained Architecture**
   - Locally hosted M3U and XML files
   - Local EPG data server
   - Integrated WebGrab+ for EPG updates
   - Custom logo/data server

2. **Automation Enhancements**
   - Automated quality selection
   - Subtitle management
   - VPN integration
   - CI/CD pipeline for updates

3. **Reliability Improvements**
   - Health monitoring
   - Automatic backup solutions
   - Service recovery mechanisms
   - Proper permission management

4. **Documentation**
   - Complete setup guides
   - Troubleshooting documentation
   - System diagrams and architecture docs
