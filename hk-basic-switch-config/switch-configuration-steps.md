# Basic Switch and End Device Configuration (Packet Tracer Lab)

This file contains the complete end-to-end console configuration for both switches (S1 and S2) and verification steps from the Packet Tracer lab.

```console
############################
# Switch S1 Configuration  #
############################

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


############################
# Switch S2 Configuration  #
############################

enable
configure terminal
hostname S2

enable secret class

line console 0
 password cisco
 login
 exit

interface vlan 1
 ip address 192.168.1.2 255.255.255.0
 no shutdown
 exit

banner motd # Unauthorized access will not be tolerated #

end
copy running-config startup-config


############################
# Verification             #
############################

# From PC-A
ping 192.168.1.11
ping 192.168.1.1
ping 192.168.1.2

# From switches
ping 192.168.1.10
ping 192.168.1.11

