# EVPN-VXLAN Fabric Lab

## Overview

Built a 2-Spine / 2-Leaf EVPN-VXLAN fabric using FRRouting and Containerlab.

Features:

- OSPF Underlay
- iBGP EVPN Overlay
- Route Reflectors
- VXLAN VNI 10010
- EVPN Type-2 and Type-3 Routes
- End-to-End Host Connectivity

## Topology

Spines

- spine1 (1.1.1.1)
- spine2 (2.2.2.2)

Leafs

- leaf1 (11.11.11.11)
- leaf2 (22.22.22.22)

Hosts

- host1 (192.168.10.11)
- host2 (192.168.10.22)

## Validation

- OSPF adjacency established
- BGP EVPN sessions established
- EVPN Type-2 MAC routes learned
- EVPN Type-3 IMET routes learned
- Successful VXLAN encapsulation
- Host-to-host ping successful

## Technologies

- FRRouting (FRR)
- Containerlab
- OSPF
- BGP
- EVPN
- VXLAN
- Linux Bridge
