# PAT (NAT Overload) Lab

## Topology
```
Linux Host (192.168.1.100)
R1 (PAT Router)
R2 (Internet)

```


## Configuration Summary
```
int g0/0 configured as NAT inside
int g0/1 configured as NAT outside
ACL 1 identifies inside addresses
PAT configured using outside interface address with overload

```


<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/nat/pat_overload/diagrams/patoverloadv1.jpg">

<br>
<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/nat/pat_overload/diagrams/patoverloadstats.jpg">
<br>
## Verification
```
show ip nat translations
show ip nat statistics

```
