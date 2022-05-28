## Net
### ss
Show only tcp sockets with tcp internal info, extended socket info, process info and memory usage in oneline
```
ss -Otiepm
```
### tcpdump
dump packet from eth0 with ip1 or ip2 to path/trace-%H with split one hour.
```
tcpdump -i eth0 -n -w path/trace-%H host {ip1} or host {ip2} -G 3600 -K
```
### sar
show network interface statistics every seconds
```
sar -n DEV 1
```
### ethtool
show nic statistics
```
ethtool -S eth0
```
show features for nic
```
ethtool -k eth0
```

## sysctl
### systeroid 
Show tui interface for manage kernel vars with their descriptions
```
systeroid --tui
```
Show detailed explanation for kernela variable
```
systeroid -E some_var
```
