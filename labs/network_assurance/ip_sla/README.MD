


### IP SLA

<br>
<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/network_assurance/ip_sla/diagrams/ipslatopology.jpg">





```
ip sla 1
icmp-echo 203.0.113.2 source-interface g0/1
frequency 5

ip sla schedule 1 life forever start-time now

show ip sla statistics
show track
```
