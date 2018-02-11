# MSI Movie Station HD1000

## Hardware
|                |Type             |Description    |
|----------------|-----------------|---------------|
|**CPU**         |MPIS 24K V7.8    |               |
|**Flash-Chip**  |HY27UF081G2A     |1GB NAND FLASH |
|**RAM**         |NT5TU64M16DG-AC  |               |
|**USB**         |2x               |               |



![teardown](https://github.com/chris0550/msi_hd1000/raw/master/images/5.jpg)


## Software

### Open ports
|PORT      |STATE |SERVICE|VERSION|
|:---------|:-----|:----------------|:-----------------------------------------|
| 23/tcp   | open | telnet          | BusyBox telnetd                          |
| 80/tcp   | open | http            | BusyBox httpd                            |
| 139/tcp  | open | netbios-ssn     | Samba smbd 3.X (workgroup: WORKGROUP)    |
| 445/tcp  | open | netbios-ssn     | Samba smbd 3.X (workgroup: WORKGROUP)    |
| 8082/tcp | open | blackice-alerts?|                                          |
| 1024/udp | open |                 |                                          |  
  

###Access
Accessible via telnet  
Username: `root`  
Password: `<not necessary>`  

![Login via telnet](https://github.com/chris0550/msi_hd1000/raw/master/images/telnet.png)

```
# uname -a
Linux Venus 2.6.12.6-VENUS #6 Mon Sep 27 11:33:46 CST 2010 mips unknown
```


```
# uname -a
# cat /proc/cpuinfo 
system type             : Realtek Venus
processor               : 0
cpu model               : MIPS 24K V7.8
BogoMIPS                : 269.51
wait instruction        : yes
microsecond timers      : yes
tlb_entries             : 32
extra interrupt vector  : yes
hardware watchpoint     : yes
ASEs implemented        : mips16
VCED exceptions         : not available
VCEI exceptions         : not available
```