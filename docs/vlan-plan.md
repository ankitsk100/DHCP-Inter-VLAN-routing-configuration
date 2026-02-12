# VLAN Plan

## VLANs
| VLAN ID | VLAN Name | Department |
|---:|---|---|
| 10 | IT | IT-DEPT |
| 20 | SALES | SALES-DEPT |
| 30 | HR | HR-DEPT |

## Trunks
- Access Switch uplinks (Fa0/4) trunk to MLS1
- MLS1 uplink trunk to R1 (Gi1/0/4 -> R1 Gi0/0)
- Allowed VLANs on trunks: 10,20,30
