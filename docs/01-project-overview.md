# Project Overview

## Project

- **Project name:** Bright Star Training Center — IT Infrastructure Design
- **Project type:** Fictional IT infrastructure planning, implementation, and cybersecurity portfolio project
- **Environment:** Three-floor training institute

## Objective

Design a practical IT infrastructure for a three-floor training center, initially covering the ground floor and second floor. The design includes wired networking, Wi-Fi, CCTV, printers, staff workstations, student computer labs, centralized connectivity, and basic network security.

## Design Approach

- Use realistic small-business networking equipment and architecture.
- Prefer wired connectivity for fixed workstations and network devices where practical.
- Provide wireless connectivity for staff, students, and guests through access points.
- Separate networks according to device function and security requirements.
- Restrict access to CCTV, network management, and other sensitive systems.
- Document the physical layout, IP addressing, configurations, security policies, and testing procedures.
- Build a working lab or simulation where practical to validate the design.

## Scope and Assumptions

- The building has three floors; the initial implementation covers the ground floor and second floor.
- A single Etisalat ISP connection is provided.
- The main rack is in the ground-floor rack room.
- Each in-scope floor has a mini rack for its network connections and equipment.
- Each computer lab has a dedicated mini rack with an unmanaged Gigabit switch.
- Existing pre-routed Ethernet cabling with RJ45 connectors will be reused.
- Two wireless access points are planned per in-scope floor.
- IP cameras connect to PoE switches, with one NVR in the ground-floor camera room.
- A NAS will provide shared storage and backup space.
- No fixed budget has been established; equipment choices should meet practical requirements without unnecessary complexity.

## Current Scope Exclusions

Patch panels, a dedicated patch-cable system, and UPS equipment are excluded from the initial design. The third floor will be added after its layout and device requirements are defined.


---

[← Previous: Documentation Home](README.md) | [Next: Building and Cabling →](02-building-and-cabling.md)