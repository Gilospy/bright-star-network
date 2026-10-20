# Building and Cabling

## Cabling Infrastructure

The building has pre-routed Ethernet cabling with RJ45 connectors. Cables from devices and rooms terminate at the corresponding floor-level or lab mini racks. Dedicated cable runs connect floor racks to the ground-floor main rack.

The design will use the existing cabling layout as its starting point. Patch panels, a dedicated patch-cable system, and UPS equipment are outside the initial design scope.

## Ground Floor

| Area / function | Requirements |
|---|---|
| Computer lab | 25 computers and one unmanaged switch |
| Office | 3 staff computers and 1 printer |
| Reception | 1 staff computer and 1 printer |
| Indoor CCTV | 7 IP cameras connected to a PoE switch |
| Outdoor CCTV | 8 outdoor cameras connected to a PoE switch |
| Camera room | 1 staff computer and 1 NVR |
| Wireless | 2 wireless access points |
| Main rack room | ISP connection, firewall/router, core and distribution switching, NAS |

## Second Floor

| Area / function | Requirements |
|---|---|
| Computer lab | 25 computers and one unmanaged switch |
| Reception | 1 staff computer and 1 printer |
| CCTV | 10 IP cameras connected to a PoE switch |
| Wireless | 2 wireless access points |

## Third Floor

The rooms, computers, staff workstations, printers, cameras, and wireless coverage for the third floor have not yet been specified. This floor is excluded from the initial implementation and will be planned when its layout is defined.

## Equipment Assumptions

| Equipment | Quantity / placement |
|---|---|
| Core managed switch | 1 at the ground-floor main rack (`SW-CORE`) |
| Distribution switches | 2: `SW-MAIN-GF` at the main rack and `SW-MAIN-L2` at the second-floor mini rack |
| Unmanaged lab switches | 1 per computer lab |
| CCTV PoE switches | 2 on the ground floor and 1 on the second floor |
| Wireless access points | 2 on the ground floor and 2 on the second floor |
| Firewall/router | 1 at the main rack |
| NVR | 1 in the camera room |
| NAS | 1 at the main rack |


---

**Navigation:** [← Project Overview](01-project-overview.md) | [Next: Network Topology →](03-network-topology.md)