## VRRP lab

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
