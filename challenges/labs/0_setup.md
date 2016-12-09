```
AMI id: DS3_V2
Region: Southeast Asia
OS: Centos 6.7
Volume Space: 28Gb
```

**YUM Repolist**
```
[root@sebcxinyi00 ~]# yum repolist enabled
Loaded plugins: fastestmirror, security
Determining fastest mirrors
base                                                     | 3.7 kB     00:00
base/primary_db                                          | 4.7 MB     00:00
extras                                                   | 3.4 kB     00:00
extras/primary_db                                        |  37 kB     00:00
openlogic                                                | 1.3 kB     00:00
openlogic/primary                                        | 286 kB     00:00
openlogic                                                                 67/67
updates                                                  | 3.4 kB     00:00
updates/primary_db                                       | 3.7 MB     00:00
repo id              repo name                                            status
base                 CentOS-6 - Base                                      6,696
extras               CentOS-6 - Extras                                       62
openlogic            CentOS-6 - openlogic packages for x86_64                67
updates              CentOS-6 - Updates                                     686
repolist: 7,511
```

**/etc/passwd**
```
raffles:x:2700:504::/home/raffles:/bin/bash
orchard:x:2800:503::/home/orchard:/bin/bash
```

**/etc/group**
```
shops:x:503:
walks:x:504:
```