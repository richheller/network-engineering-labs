## VRRP lab

<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/fhrp/vrrp/diagrams/vrrpv.jpg">
<br>

### Server config
```
sudo ifconfig eth0 203.0.113.2 netmask 255.255.255.0 up
sudo route add default gw 203.0.113.1 

```
### Linux host config
```
ip addr add 192.168.1.100/24 dev eth0
ip route add default via 192.168.1.1
```
<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/fhrp/vrrp/diagrams/r1vrrpbrief.jpg">
<br>
<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/fhrp/vrrp/diagrams/r2vvrpbrief.jpg">
<br>
<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/fhrp/vrrp/diagrams/r1shutvrrp.jpg">
<br>
<img src="https://github.com/richheller/network-engineering-labs/blob/main/labs/fhrp/vrrp/diagrams/R2nowmaster.jpg">
