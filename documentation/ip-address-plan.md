# IP Address Plan

This page explains the simulated IP and VLAN structure used in this network documentation lab.

The source table is available in [`data/ip_address_plan.csv`](../data/ip_address_plan.csv).

## Network Segments

| VLAN | Name | Subnet | Purpose |
|---:|---|---|---|
| 10 | Management | 192.168.10.0/24 | Network device administration |
| 20 | Corporate Users | 192.168.20.0/24 | Office workstations and laptops |
| 30 | Shared Services | 192.168.30.0/24 | Shared business systems and internal services |
| 40 | Camera Network | 192.168.40.0/24 | Site camera and recording devices |
| 50 | Guest Wi-Fi | 192.168.50.0/24 | Guest internet access |
| 60 | Facilities Devices | 192.168.60.0/24 | Printers, scanners, and facility devices |

## Documentation Notes

- Keep device names consistent across the IP plan, switch port map, and patch panel map.
- Reserve lower IP ranges for infrastructure devices and static assignments.
- Use DHCP for standard user devices where appropriate.
- Place cameras, printers, and facility devices into documented network segments.
- Update this document whenever a new VLAN, device group, or subnet is added.

## IT Support Relevance

A clear IP address plan helps support staff troubleshoot connectivity issues, identify device ownership, avoid duplicate addressing, and understand which device groups belong to which network segment.
