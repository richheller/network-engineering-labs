

# GRE Tunnel with OSPF

<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/overlays/gre_ospf_tunnel/diagrams/gre_tunnel.jpg">

## Objective 
Configure and verify a GRE tunnel between two routers and establish an OSPF adjacency across the tunnel.

## Verification

-Tunnel0 up/up
-OSPF neighbor state FULL
-Reachability between loopbacks

## Key Commands
```
show interface tunnel0
sh ip ospf neighbor
sh ip route ospf
```
