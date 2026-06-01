
### HSRP Lab
<Br>
<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/fhrp/hsrp/hsrp_failover/diagrams/topology.png?raw=true">
<br>
<h3>Linux host configuration</h3><br><br>

ip address 192.168.1.100/24<br><br>

commands<br>
ip addr add 192.168.1.100/24 dev eth0<br>
ip route add default via 192.168.1.254<br>

<Br>



<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/fhrp/hsrp/hsrp_failover/diagrams/R1standby.jpg">




<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/fhrp/hsrp/hsrp_failover/diagrams/R2standby.jpg">


<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/fhrp/hsrp/hsrp_failover/diagrams/R1shut.jpg">


<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/fhrp/hsrp/hsrp_failover/diagrams/R2%20active.jpg">
<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/fhrp/hsrp/hsrp_failover/diagrams/R2active.jpg">



<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/fhrp/hsrp/hsrp_failover/diagrams/testingpreempt.jpg">
