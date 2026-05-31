# EVPN-VXLAN Lab

## Topology

spine1 (1.1.1.1)

spine2 (2.2.2.2)

leaf1 (11.11.11.11)

leaf2 (22.22.22.22)

host1 (192.168.10.11)

host2 (192.168.10.22)

## Underlay

OSPF Area 0

## Overlay

iBGP AS 65000

Route Reflectors:

- spine1

- spine2

## EVPN

address-family l2vpn evpn

advertise-all-vni

VNI 10010

## VXLAN

leaf1 VTEP: 11.11.11.11

leaf2 VTEP: 22.22.22.22

vxlan10010

## Validation

show ip ospf neighbor

show bgp summary

show bgp l2vpn evpn summary

show evpn vni

host1 -> host2 ping successful

0% packet loss
