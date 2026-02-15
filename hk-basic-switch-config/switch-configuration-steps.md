S1 — Complete configuration (lab)
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


S2 — Complete configuration (lab)

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
