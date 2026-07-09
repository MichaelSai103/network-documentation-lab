# Patch Panel Map

This document maps simulated patch panel ports to wall outlets, switch ports, VLANs, and physical areas.

The source table is available in [`data/patch_panel_map.csv`](../data/patch_panel_map.csv).

## Purpose

Patch panel documentation is important for onsite IT support because it helps trace physical connectivity from the rack to the user or device location.

It is especially useful for:

- New site setup
- Office desk moves
- Warehouse device relocation
- Cable fault investigation
- Network handover documentation
- Identifying unused or spare ports

## Example Mapping

| Patch Panel | Port | Wall Outlet | Switch | Switch Port | VLAN | Area |
|---|---:|---|---|---|---|---|
| PP-A | 01 | OFF-01 | SW-OFFICE-01 | Gi1/0/1 | 20 | Office Desk 1 |
| PP-A | 02 | OFF-02 | SW-OFFICE-01 | Gi1/0/2 | 20 | Office Desk 2 |
| PP-A | 04 | OFF-04 | SW-OFFICE-01 | Gi1/0/6 | 60 | Office Printer Area |
| PP-B | 01 | WH-01 | SW-WAREHOUSE-01 | Gi1/0/1 | 40 | Warehouse Entry |
| PP-B | 03 | WH-03 | SW-WAREHOUSE-01 | Gi1/0/3 | 20/50 | Warehouse Ceiling |

## Documentation Rules

- Use consistent labels for patch panel ports and wall outlets.
- Keep the switch port map and patch panel map aligned.
- Mark spare ports clearly.
- Update documentation when cables are moved or repatched.
- Avoid using undocumented temporary patches for long-term production use.

## IT Support Relevance

A clear patch panel map reduces troubleshooting time and supports reliable handover between field technicians, service desk staff, and network support teams.
