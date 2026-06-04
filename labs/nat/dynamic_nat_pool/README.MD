## Dynamic NAT


<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/nat/dynamic_nat_pool/diagrams/dynnattopology.jpg">

### Objective
Configure dynamic NAT using a public address pool and verify address allocation for multiple inside hosts.

<br>
Three inside hosts were dynamically assigned public IP addresses from INTERNET_POOL.

### Verification
```
show run | section ip nat
show access-lists
show ip nat translations
show ip nat statistics
```

Results
<br>
- Three inside hosts successfully reached the server<br>
- Dynamic translations were allocated from INTERNET_POOL<br>
- NAT statistics confirmed pool utilization<br>
- End-to-end connectivity verified<br>

<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/nat/dynamic_nat_pool/diagrams/secipnat.jpg">

<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/nat/dynamic_nat_pool/diagrams/sh_access-lists.jpg">

<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/nat/dynamic_nat_pool/diagrams/intg00.jpg">
<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/nat/dynamic_nat_pool/diagrams/intg01.jpg">
<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/nat/dynamic_nat_pool/diagrams/dynnattrans.jpg">
<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/nat/dynamic_nat_pool/diagrams/dynatstats.jpg">
<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/nat/dynamic_nat_pool/diagrams/pingresult.jpg">
<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/nat/dynamic_nat_pool/diagrams/shiprouteconnect.jpg">



