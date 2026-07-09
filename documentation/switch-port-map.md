# Switch Port Map

This page documents how simulated access switch ports are assigned to uplinks, user devices, cameras, wireless access points, printers, and facility devices.

The source table is available in [`data/switch_port_map.csv`](../data/switch_port_map.csv).

## Purpose

A switch port map helps IT support teams:

- Identify what is connected to each switch port
- Troubleshoot connectivity issues faster
- Understand which VLAN or segment a device belongs to
- Support moves, adds, and changes
- Maintain accurate handover documentation

## Example Port Mapping

| Switch | Port | Connected To | Device Type | VLAN | Location |
|---|---|---|---|---|---|
| SW-CORE-01 | Gi1/0/1 | EDGE-GW-01 | Uplink | Trunk | Server Room |
| SW-CORE-01 | Gi1/0/2 | SW-OFFICE-01 | Uplink | Trunk | Server Room |
| SW-CORE-01 | Gi1/0/3 | SW-WAREHOUSE-01 | Uplink | Trunk | Server Room |
| SW-OFFICE-01 | Gi1/0/3 | AP-OFFICE-01 | Wireless AP | 20/50 | Office Ceiling |
| SW-WAREHOUSE-01 | Gi1/0/1 | CAM-WH-01 | Camera | 40 | Warehouse Entry |

## Documentation Rules

- Label uplinks clearly.
- Record patch panel references where possible.
- Note whether a port is used for user devices, camera devices, wireless access points, or shared equipment.
- Keep port labels consistent with device labels and physical rack labels.
- Update the map after any port move or device replacement.

## Troubleshooting Value

When a user reports an issue, the port map helps support staff trace the affected endpoint from wall outlet to patch panel, switch port, VLAN, and upstream path.
