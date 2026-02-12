# Verification

## Router (R1)
Run:
- `show ip interface brief`
- `show run interface g0/0.10`
- `show run interface g0/0.20`
- `show run interface g0/0.30`
- `show ip dhcp pool`
- `show ip dhcp binding`

Expected:
- Subinterfaces are **up/up**
- DHCP pools show **active** and bindings appear after PCs request DHCP

## Switches
Run:
- `show vlan brief`
- `show interfaces trunk`

Expected:
- VLANs exist and access ports are in the correct VLAN
- Trunk ports show VLANs 10,20,30 allowed and forwarding
