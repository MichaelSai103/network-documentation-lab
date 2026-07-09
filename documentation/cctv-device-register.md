# Camera Device Register

This document records simulated site camera and recording devices for a small office and warehouse environment.

The source table is available in [`data/cctv_device_register.csv`](../data/cctv_device_register.csv).

## Purpose

A camera device register helps support teams understand:

- Where each camera is installed
- Which switch and port it connects to
- Which network segment it belongs to
- Whether it uses PoE or another power source
- Which recording system receives the stream
- What area each device is intended to cover

## Example Register

| Device ID | Type | Location | Network Segment | Switch | Port | Recording Target |
|---|---|---|---|---|---|---|
| CAM-WH-01 | IP camera | Warehouse Entry | Camera Network | SW-WAREHOUSE-01 | Gi1/0/1 | NVR-01 |
| CAM-WH-02 | IP camera | Warehouse Packing Area | Camera Network | SW-WAREHOUSE-01 | Gi1/0/2 | NVR-01 |
| CAM-OFF-01 | IP camera | Office Reception | Camera Network | SW-OFFICE-01 | Gi1/0/7 | NVR-01 |
| CAM-EXT-01 | IP camera | External Loading Area | Camera Network | SW-WAREHOUSE-01 | Gi1/0/5 | NVR-01 |
| NVR-01 | Network video recorder | Server Room | Shared Services | SW-CORE-01 | Gi1/0/4 | N/A |

## Support Notes

When a camera is offline, support staff should check:

- Whether the device is powered
- Whether the connected switch port is active
- Whether the patch panel and wall outlet labels match the documentation
- Whether the device appears in the expected network segment
- Whether the recording system can receive the device stream
- Whether recent physical work may have affected cabling

## Portfolio Relevance

This document reflects practical field support documentation for site infrastructure, camera systems, and network-connected devices.
