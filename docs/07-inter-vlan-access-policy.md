# Inter-VLAN Access Policy

## Legend

- **A — Allowed:** Communication is permitted where required.
- **D — Denied:** Communication is not permitted.
- **L — Limited:** Communication is permitted only for specified services or operational requirements.

## Inter-VLAN Policy Matrix

| Source ↓ / Destination → | Staff 10 | Students 20 | CCTV 30 | Resources 40 | Guest 50 | Management 60 |
|---|---:|---:|---:|---:|---:|---:|
| Staff 10 | A | L | L | A | D | D |
| Students 20 | D | A | D | D | D | D |
| CCTV 30 | D | D | A | D | D | D |
| Resources 40 | D | D | D | A | D | D |
| Guest 50 | D | D | D | D | A | D |
| Management 60 | L | L | L | L | D | A |

## Internet Access Policies

| Traffic | Policy |
|---|---|
| Staff → Internet | Allow |
| Students → Internet | Allow |
| CCTV → Internet | Deny by default |
| Staff Resources → Internet | Limited |
| Guest → Internet | Allow |
| Management → Internet | Limited |

## Policy Notes

- Staff access to shared printers and NAS storage is permitted; NAS account permissions also apply.
- Student and guest access to restricted internal resources is denied.
- Access to the NVR and network management interfaces is limited to authorized devices and administrators.
- The exact services permitted by each **Limited** rule should be defined when firewall rules are implemented.

---

**Navigation:** [← Network Services](06-network-services.md) | [Next: Testing and Validation →](08-testing-and-validation.md)