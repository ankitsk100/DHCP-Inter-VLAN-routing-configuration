# Addressing Plan

## VLAN Subnets
| VLAN | Name | Subnet | Gateway | DHCP Excluded |
|---:|---|---|---|---|
| 10 | IT | 192.168.1.0/24 | 192.168.1.1 | 192.168.1.1–192.168.1.10 |
| 20 | SALES | 192.168.2.0/24 | 192.168.2.1 | 192.168.2.1–192.168.2.10 |
| 30 | HR | 192.168.3.0/24 | 192.168.3.1 | 192.168.3.1–192.168.3.10 |

## Notes
- Default gateways are configured on router subinterfaces (Router-on-a-Stick).
- Clients receive IP addresses dynamically via DHCP from R1.
