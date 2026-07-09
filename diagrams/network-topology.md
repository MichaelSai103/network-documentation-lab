# Network Topology

This page uses Mermaid to show the simulated network topology for the office and warehouse site.

```mermaid
flowchart TB
    Internet((Internet))
    Edge[Edge Gateway]
    Core[SW-CORE-01\nCore Switch]
    Office[SW-OFFICE-01\nOffice Access Switch]
    Warehouse[SW-WAREHOUSE-01\nWarehouse Access Switch]

    NVR[NVR-01\nRecording System]
    Server[Shared Services]
    Printer[PRN-OFFICE-01\nShared Printer]
    OfficeAP[AP-OFFICE-01\nOffice Wi-Fi]
    WarehouseAP[AP-WH-01\nWarehouse Wi-Fi]
    Users[Office Workstations]
    Cameras[Warehouse / Office Cameras]
    Facility[Facility Devices]

    Internet --> Edge --> Core
    Core --> Office
    Core --> Warehouse
    Core --> NVR
    Core --> Server
    Office --> Users
    Office --> OfficeAP
    Office --> Printer
    Warehouse --> WarehouseAP
    Warehouse --> Cameras
    Warehouse --> Facility
```

## Reading the Diagram

- The edge gateway connects the site to the outside network.
- The core switch connects the main site segments.
- Office and warehouse access switches connect local endpoints.
- Site camera devices and facility devices are documented separately from user workstations.
- Shared services and recording equipment are placed in the server room / communications rack.

## Notes

This is a simulated topology for documentation practice. It does not represent any real company network.
