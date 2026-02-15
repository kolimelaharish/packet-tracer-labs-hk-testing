# Basic Switch and End Device Configuration (Packet Tracer)

This file describes the complete setup and configuration of a basic LAN using two switches and two PCs in Cisco Packet Tracer.

I completed a basic networking lab in Cisco Packet Tracer where I configured two switches and two PCs in a small LAN topology.

First, I performed the physical setup by placing the switches in the rack and the PCs on the table, and I connected the devices using the correct cable types — a copper cross-over cable between the two switches and copper straight-through cables between each PC and its switch.

Then I configured the IP addressing plan based on the lab table, assigning IP addresses to PC-A, PC-B, and the VLAN 1 interfaces of switches S1 and S2.

After that, I accessed each switch using a console connection and configured the hostname, console password, enable secret, MOTD banner, and the VLAN 1 management IP address.

Finally, I verified connectivity using ping between PCs and switches. All tests were successful, and the Packet Tracer assessment showed 100% completion.

This lab demonstrates basic racking, cabling, IP addressing, and initial switch configuration in a small LAN.

```console
Lab Overview
------------
I completed a basic networking lab in Cisco Packet Tracer where I configured two switches and two PCs in a small LAN topology.


Physical Setup
--------------
Rack:
  Switch S1 and Switch S2 placed in rack

Workspace:
  PC-A and PC-B placed on table

Cabling:
  Copper cross-over cable between S1 and S2
  Copper straight-through cable between PC-A and S1
  Copper straight-through cable between PC-B and S2


IP Addressing Plan
------------------
PC-A        : 192.168.1.10 /24
PC-B        : 192.168.1.11 /24
S1 VLAN 1   : 192.168.1.1 /24
S2 VLAN 1   : 192.168.1.2 /24


Switch Configuration
--------------------
Access:
  Console connection from PC to each switch

Configured on both switches:
  Hostname
  Console password
  Enable secret
  MOTD banner
  VLAN 1 management IP address


Connectivity Verification
-------------------------
Ping between PCs and switches

Result:
  All tests successful
  Packet Tracer assessment: 100%


Skills Demonstrated
-------------------
Basic racking
Ethernet cabling
IP addressing
Initial Cisco switch configuration
Small LAN connectivity
