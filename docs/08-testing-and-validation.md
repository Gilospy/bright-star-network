# Testing and Validation Plan

## Purpose

This plan defines the checks to perform after implementation. The objective is to confirm that devices receive the correct network settings, required services are accessible, and network segmentation behaves as intended.

## Connectivity Testing

- Verify that each VLAN receives addresses from the correct subnet and DHCP scope.
- Confirm that devices can reach their assigned default gateway.
- Verify connectivity between network devices and required infrastructure services.
- Confirm that authorized clients can access the internet where permitted.

## Inter-VLAN Access Testing

- Confirm that staff devices can access designated shared resources.
- Verify that student and guest devices cannot access restricted internal networks.
- Confirm that CCTV devices can communicate with the NVR as required.
- Verify that network management interfaces are accessible only from authorized administrative devices.
- Confirm that prohibited inter-VLAN communication is blocked.

## Network Services Testing

- Verify that DHCP assigns the correct IP address, subnet mask, and default gateway.
- Test authorized access to NAS storage and network printers.
- Verify that the NVR receives video from the designated cameras.

## Documentation and Results

Record the expected result, observed result, and pass/fail status for each test. Investigate failed tests, apply corrective actions, and retest.

The validation process will help confirm that the implemented network meets the requirements established during planning.

---

**Navigation:** [← Access Policy](07-inter-vlan-access-policy.md) | [Documentation Home →](README.md)