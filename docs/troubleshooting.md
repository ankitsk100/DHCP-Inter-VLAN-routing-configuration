# Troubleshooting

## PC not getting DHCP address
Check:
1. Trunks are up:
   - `show interfaces trunk`
2. VLAN exists on each switch:
   - `show vlan brief`
3. Router subinterfaces are up:
   - `show ip interface brief`
4. DHCP pools exist:
   - `show ip dhcp pool`

Common fixes:
- Ensure uplink port is trunk on BOTH ends
- Ensure allowed VLAN list includes 10,20,30
- Ensure router physical interface has `no ip address` and is `no shutdown`

## VLAN works locally but no inter-VLAN connectivity
- Confirm subinterface encapsulation:
  - `encapsulation dot1Q <vlan-id>`
- Confirm gateway IP matches VLAN subnet
