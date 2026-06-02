


### IP SLA

<br>
<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/network_assurance/ip_sla/diagrams/ipslatopology.jpg">

### Objective
Configure IP SLA on R1 to continuosly monitor reachability of 203.0.113.2.
SLA operation performs an ICMP echo every 5 seconds and is tied to a track object.
When connectivity is interrupted, track object changes state from Up to Down.


#### commands
```
ip sla 1
icmp-echo 203.0.113.2 source-interface g0/1
frequency 5

ip sla schedule 1 life forever start-time now

show ip sla statistics
show track
```
<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/network_assurance/ip_sla/diagrams/ipslastats1.jpg">
<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/network_assurance/ip_sla/diagrams/shtrack1.jpg">
<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/network_assurance/ip_sla/diagrams/shslastatistics.jpg">
<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/network_assurance/ip_sla/diagrams/shutdown.jpg">

<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/network_assurance/ip_sla/diagrams/result.jpg">
