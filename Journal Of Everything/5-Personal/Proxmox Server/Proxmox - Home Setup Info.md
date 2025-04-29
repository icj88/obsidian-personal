Local address: 192.168.1.16 #TODO make this gets turned into a static IP ASAP!!!
Default Username: root
Default Password: standard format with initialization

# Network info
Name: vmbr0
Type: linux bridge
Active: Yes
VLAN Aware: No
Ports/Slaves: eno3
CIDR: 192.168.1.16/24
Gateway: 192.168.1.1

```
ip a
1: lo: <LOOPBACK,UP,LOWER_UP> mtu 65536 qdisc noqueue state UNKNOWN group default qlen 1000
    link/loopback 00:00:00:00:00:00 brd 00:00:00:00:00:00
    inet 127.0.0.1/8 scope host lo
       valid_lft forever preferred_lft forever
    inet6 ::1/128 scope host noprefixroute 
       valid_lft forever preferred_lft forever
2: eno3: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc mq master vmbr0 state UP group default qlen 1000
    link/ether 24:6e:96:35:65:9c brd ff:ff:ff:ff:ff:ff
    altname enp6s0f0
3: eno4: <BROADCAST,MULTICAST> mtu 1500 qdisc noop state DOWN group default qlen 1000
    link/ether 24:6e:96:35:65:9d brd ff:ff:ff:ff:ff:ff
    altname enp6s0f1
4: eno1: <BROADCAST,MULTICAST> mtu 1500 qdisc noop state DOWN group default qlen 1000
    link/ether 24:6e:96:35:65:98 brd ff:ff:ff:ff:ff:ff
    altname enp1s0f0
5: eno2: <BROADCAST,MULTICAST> mtu 1500 qdisc noop state DOWN group default qlen 1000
    link/ether 24:6e:96:35:65:9a brd ff:ff:ff:ff:ff:ff
    altname enp1s0f1
6: vmbr0: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc noqueue state UP group default qlen 1000
    link/ether 24:6e:96:35:65:9c brd ff:ff:ff:ff:ff:ff
    inet 192.168.1.16/24 scope global vmbr0
       valid_lft forever preferred_lft forever
    inet6 fe80::266e:96ff:fe35:659c/64 scope link 
       valid_lft forever preferred_lft forever
```
