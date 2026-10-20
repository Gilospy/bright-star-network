# Wireless Network Design

## Access Point Requirements and Placement

Four wireless access points will be deployed across the two in-scope floors, with two access points per floor. The initial placement will be near opposite corners of each floor to provide coverage across the building. Placement and transmit power should be checked through coverage testing.

Each access point connects to the managed network infrastructure through Ethernet. Its switch port carries the required VLANs using VLAN tagging.

## SSID and VLAN Mapping

Each access point will broadcast three wireless networks (SSIDs).

| SSID | VLAN ID | Access |
|---|---:|---|
| Bright Star Staff | 10 | Staff network and authorized internal resources |
| Bright Star Students | 20 | Student network and internet |
| Bright Star Guest | 50 | Internet only |

## Wireless Security

- All three SSIDs will use WPA2-Personal with AES encryption.
- Each SSID will have its own password.
- Guest credentials will be kept separate from staff and student credentials.
- Guest devices will be restricted to internet access.
- Access point management interfaces will reside on VLAN 60 and be accessible only to authorized IT administrators.

## Initial Radio Settings

| Setting | Proposed configuration |
|---|---|
| Frequency band | 5 GHz only |
| Channel width | 20 MHz |
| Channel selection | Assign different, non-overlapping channels to nearby access points where possible |
| Transmit power | Medium initially; adjust after coverage testing |
| SSID broadcasting | Three SSIDs per access point |
| Security | WPA2-Personal (AES) |


---

**Navigation:** [← VLAN and IP Plan](04-vlan-and-ip-plan.md) | [Next: Network Services →](06-network-services.md)