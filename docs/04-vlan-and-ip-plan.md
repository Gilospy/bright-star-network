# VLAN and IP Addressing Plan

## VLAN Design

VLANs separate devices into logical network segments based on function. Communication between VLANs will be controlled by the firewall/router.

| VLAN ID | VLAN name | Purpose |
|---:|---|---|
| 10 | Staff | Staff PCs and staff wireless devices |
| 20 | Students | Student lab PCs and student wireless devices |
| 30 | CCTV | IP cameras and the Network Video Recorder (NVR) |
| 40 | Staff Resources | Shared network printers and NAS storage |
| 50 | Guest Wi-Fi | Visitor wireless access, restricted to internet access |
| 60 | Network Management | Management interfaces for switches and wireless access points |

## VLAN Access Principles

- Staff devices can access shared printers and the NAS, subject to NAS account permissions.
- Student devices are restricted from staff resources, network management interfaces, and CCTV equipment.
- Guest devices are restricted to internet access and cannot access internal network resources.
- Access to the NVR is restricted to authorized devices and users through firewall rules and NVR account permissions.
- Network management interfaces are accessible only to authorized IT administrators.
- The firewall/router provides the default gateway for each VLAN and controls inter-VLAN communication.
- Staff PCs and staff Wi-Fi use the same Staff VLAN. Access points map SSIDs to their corresponding VLANs.

## IP Addressing Plan

The proposed private address block is `192.168.0.0/22`. VLSM is used to allocate subnets according to expected device counts.

| VLAN ID | Name | Network | Gateway |
|---:|---|---|---|
| 50 | Guest Wi-Fi | `192.168.0.0/24` | `192.168.0.1` |
| 20 | Students | `192.168.1.0/24` | `192.168.1.1` |
| 10 | Staff | `192.168.2.0/25` | `192.168.2.1` |
| 30 | CCTV | `192.168.2.128/26` | `192.168.2.129` |
| 40 | Staff Resources | `192.168.2.192/27` | `192.168.2.193` |
| 60 | Network Management | `192.168.3.0/27` | `192.168.3.1` |

These subnets are non-overlapping and fit within `192.168.0.0/22`.

## DHCP and Static IP Allocation

DHCP will assign addresses to staff, student, and guest clients. Devices that require predictable addresses will use static IP addresses or DHCP reservations.

| Device type | VLAN | Address assignment |
|---|---|---|
| Staff and student devices | Staff / Students | DHCP |
| Guest wireless devices | Guest Wi-Fi | DHCP |
| Switches and access points | Network Management | Static IP or DHCP reservation |
| IP cameras and NVR | CCTV | Static IP or DHCP reservation |
| Network printers and NAS | Staff Resources | Static IP or DHCP reservation |
| VLAN gateways | All VLANs | Fixed IP addresses |

---

**Navigation:** [← Network Topology](03-network-topology.md) | [Next: Wireless Design →](05-wireless-design.md)