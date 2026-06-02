

# GRE Tunnel with OSPF

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
