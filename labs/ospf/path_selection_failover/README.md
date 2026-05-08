
# OSPF Path Selection

## under construction



- OSPF neighbor adjacency
- SPF path selection


<br>



<br>



### Introduction

Open Shortest Path First (OSPF) routing protocol is an open-source link state routing protocol. OSPF routers run the Dijistra shortest path first (SPF) algorithm to calculate lowest path cost through the network.

Reference: Cisco CCNP and CCIE Enterprise Core ENCOR 350-401 Official Cert Guide

I created this topology from scratch on a server I host myself running CML.

## Topology


  <img width="950" height="423" alt="image" src="https://github.com/user-attachments/assets/922e5f58-ee8b-48cf-be34-afb16f902b7d" />


### configure OSPF, form adjacencies 
setting loopback 0 interfaces to 1.1.1.1, 2.2.2.2 etc.
 OSPF networks

<img width="753" height="128" alt="image" src="https://github.com/user-attachments/assets/e206eba6-731e-44f8-9268-3891d17202ad" />


### check existing ip route


<img width="637" height="577" alt="image" src="https://github.com/user-attachments/assets/f4aeef3d-89d9-4e39-8758-f053d9507315" />

sh ip route to 4.4.4.4 
<img width="541" height="163" alt="image" src="https://github.com/user-attachments/assets/1e4a1e5a-6e55-4f82-8cdc-e2283a874474" />


<br><Br>
Initialy, path selection to R4 is direct to R4 via 10.0.14.0/30 to 10.0.14.2.
<br><Br>
<img width="351" height="115" alt="image" src="https://github.com/user-attachments/assets/78c6443b-e08e-4e56-8659-40ff019f3d77" />

<Br>
<img width="806" height="263" alt="image" src="https://github.com/user-attachments/assets/d6aaa040-a3c0-4804-8e46-d8d72f760ba2" />
<br><br>

Next, the OSPF cost on the direct R1 to R4 path is increased to influence SPF path selection.


## image


After the cost change, OSPF recalculates the topology and selects the lower-cost-path through R2.


