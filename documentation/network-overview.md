# Network Overview

This document describes a simulated small office and warehouse network. The environment is for portfolio demonstration only and does not represent any real company site.

## Scenario

The site contains:

- One small office area
- One warehouse area
- A server room / communications rack
- Corporate wired and wireless users
- Guest Wi-Fi
- Shared services
- Site cameras and recording equipment
- Printers and facility devices

## Documentation Goals

The purpose of this lab is to demonstrate practical IT support and junior network support documentation, including:

- Network topology documentation
- VLAN and IP address planning
- Switch port mapping
- Patch panel and wall outlet mapping
- Site camera register
- Basic troubleshooting notes
- Handover-style documentation for ongoing support

## High-Level Design

The simulated network uses an edge gateway connected to a core switch. The core switch connects to separate office and warehouse access switches. Endpoints are grouped into different network segments for management, corporate users, shared services, camera devices, guest Wi-Fi, and facilities devices.

## Support Assumptions

- Network devices are labelled and documented.
- Patch panel ports are mapped to wall outlets and switch ports.
- Camera and facility devices are placed in dedicated network segments.
- Guest Wi-Fi is kept separate from corporate devices.
- Shared services are placed in a dedicated service segment.
- Documentation should be updated whenever ports, devices, or locations change.

## Portfolio Relevance

This project is relevant to IT Support, Field IT Support, Desktop Support, Junior Network Support, and Technical Support roles because it demonstrates practical documentation that is often required during site setup, support handover, troubleshooting, and network administration.
