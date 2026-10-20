# Network Services

## Overview

The network will provide centralized services for staff, students, shared resources, CCTV, and network administration. Services will use appropriate IP addresses and be accessible only to the network segments that require them.

## DHCP

Dynamic Host Configuration Protocol (DHCP) will automatically assign IP addresses and other network settings to client devices. Separate DHCP scopes will be maintained for applicable VLANs, using the corresponding subnet and default gateway.

Devices requiring predictable addresses, including network infrastructure, the NAS, and the NVR, will use static addresses or DHCP reservations.

## Network-Attached Storage

A Network-Attached Storage (NAS) device will provide shared file storage and a location for backups. Access will be restricted to authorized users and devices according to the intended access policy.

## CCTV Recording

A Network Video Recorder (NVR) will centrally record footage from the building's IP cameras. Cameras will communicate with the NVR over the designated CCTV network, with access to other network segments restricted.

## Network Management

Network infrastructure will be managed through designated administrative access. Management interfaces will not be generally accessible to student or guest devices.

---

**Navigation:** [← Wireless Design](05-wireless-design.md) | [Next: Access Policy →](07-inter-vlan-access-policy.md)