# Cisco_Packets
NAT Command
interface Fa0/0
ip nat inside
exit
interface Fa0/1
ip nat outside
exit


OSPF Commmand 
(Router 0)
router ospf 10
network 192.168.10.0 0.0.0.255 area 0
network 192.168.30.0 0.0.0.255 area 0
end

(Router 1)
router ospf 10
network 192.168.30.0 0.0.0.255 area 0
network 192.168.20.0 0.0.0.255 area 0
end
