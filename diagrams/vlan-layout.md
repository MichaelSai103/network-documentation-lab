# VLAN Layout

This page shows the simulated VLAN layout used in the network documentation lab.

```mermaid
flowchart LR
    Core[Core Switch]

    V10[VLAN 10\nManagement\n192.168.10.0/24]
    V20[VLAN 20\nCorporate Users\n192.168.20.0/24]
    V30[VLAN 30\nShared Services\n192.168.30.0/24]
    V40[VLAN 40\nCamera Network\n192.168.40.0/24]
    V50[VLAN 50\nGuest Wi-Fi\n192.168.50.0/24]
    V60[VLAN 60\nFacilities Devices\n192.168.60.0/24]

    Core --> V10
    Core --> V20
    Core --> V30
    Core --> V40
    Core --> V50
    Core --> V60
```

## VLAN Summary

| VLAN | Name | Purpose |
|---:|---|---|
| 10 | Management | Network device administration |
| 20 | Corporate Users | Office workstations and laptops |
| 30 | Shared Services | Shared business systems and internal services |
| 40 | Camera Network | Site camera and recording devices |
| 50 | Guest Wi-Fi | Guest internet access |
| 60 | Facilities Devices | Printers, scanners, and facility devices |

## Support Notes

- VLAN documentation should be consistent with the IP address plan.
- Device labels should match the switch port map and patch panel map.
- Guest Wi-Fi and user devices should be documented as separate service groups.
- Camera and facility devices should be easy to identify for onsite troubleshooting.
