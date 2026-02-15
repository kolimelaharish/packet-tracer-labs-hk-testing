# Basic Switch and End Device Configuration (Packet Tracer Lab)

This file contains the complete switch configurations and verification commands for switches S1 and S2 based on the Packet Tracer lab.

---

## **S1 — Complete Configuration**

```console
enable
configure terminal

hostname S1

enable secret class

line console 0
 password cisco
 login
 exit

interface vlan 1
 ip address 192.168.1.1 255.255.255.0
 no shutdown
 exit

banner motd # Unauthorized access will not be tolerated #

end
copy running-config startup-config
