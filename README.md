# Bright Star Training Center — Network Design & Implementation

## Overview

This project focuses on designing, simulating, and implementing a segmented network for a three-floor training center using GNS3 and OPNsense.

The initial scope covers the ground floor and second floor, with the third floor reserved for future expansion.

## Objectives

- Design a physical and logical network topology.
- Implement VLAN-based network segmentation.
- Develop an IP addressing plan using VLSM.
- Configure DHCP and DNS services.
- Define inter-VLAN access policies.
- Simulate and validate connectivity in GNS3.
- Document configurations, testing, and troubleshooting.

## Planned Technologies

- **GNS3** — Network simulation
- **OPNsense** — Firewall and network routing
- **VLANs** — Network segmentation
- **DHCP and DNS** — Client network services
- **NAS and CCTV/NVR** — Shared storage and surveillance infrastructure

## Network Segmentation

| VLAN | Purpose |
|---|---|
| VLAN 10 | Staff |
| VLAN 20 | Students |
| VLAN 30 | CCTV |
| VLAN 40 | Staff Resources |
| VLAN 50 | Guest Wi-Fi |
| VLAN 60 | Network Management |

See the detailed documentation for subnet allocations, gateways, and access policies.

## Network Topology

Physical and logical topology diagrams will be added as the design is finalized.

## Documentation

Detailed planning documents, diagrams, configurations, and test results will be organized in their respective directories as the project progresses.

## Project Status

**Current phase:** Design and planning

Implementation and validation will be documented as the GNS3 lab is developed.

