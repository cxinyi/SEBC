**1. Check vm.swappiness**

[hduser@SEBCxinyi ~]$ cat /proc/sys/vm/swappiness

1



**2. Show the mount attributes of all volumes**

[hduser@SEBCxinyi ~]$ mount -l
/dev/sda2 on / type ext4 (rw)
proc on /proc type proc (rw)
sysfs on /sys type sysfs (rw)
devpts on /dev/pts type devpts (rw,gid=5,mode=620)
tmpfs on /dev/shm type tmpfs (rw)
/dev/sda1 on /boot type ext4 (rw)
/dev/sda3 on /var type ext4 (rw)
none on /proc/sys/fs/binfmt_misc type binfmt_misc (rw)
/dev/sdb1 on /mnt/resource type ext4 (rw)



**3. Show the reserve space of any non-root, ext-based volumes**

[hduser@SEBCxinyi ~]$ df -h
Filesystem      Size  Used Avail Use% Mounted on
/dev/sda2        20G  2.0G   18G  10% /
tmpfs           6.9G     0  6.9G   0% /dev/shm
/dev/sda1       488M   93M  370M  21% /boot
/dev/sda3        29G  172M   28G   1% /var
/dev/sdb1        28G   44M   26G   1% /mnt/resource



**4. Show that transparent hugepages is disabled**

[hduser@SEBCxinyi ~]$ sudo vi /etc/rc.local
#!/bin/sh
#
# This script will be executed *after* all the other init scripts.
# You can put your own initialization stuff in here if you don't
# want to do the full Sys V style init stuff.

touch /var/lock/subsys/local
for i in `ls /sys/block/sd*/queue/scheduler`
do
echo "noop" > $i
done
echo never > /sys/kernel/mm/redhat_transparent_hugepage/enabled
echo never > /sys/kernel/mm/redhat_transparent_hugepage/defrag


[hduser@SEBCxinyi ~]$ cat /proc/sys/vm/nr_hugepages
0



**5. Report the network interface attributes**

[hduser@SEBCxinyi ~]$ ifconfig
eth0      Link encap:Ethernet  HWaddr 00:0D:3A:A2:AE:5A
          inet addr:172.16.7.7  Bcast:172.16.7.255  Mask:255.255.255.0
          UP BROADCAST RUNNING MULTICAST  MTU:1500  Metric:1
          RX packets:21950 errors:0 dropped:0 overruns:0 frame:0
          TX packets:25248 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:1000
          RX bytes:4335911 (4.1 MiB)  TX bytes:3956625 (3.7 MiB)

lo        Link encap:Local Loopback
          inet addr:127.0.0.1  Mask:255.0.0.0
          UP LOOPBACK RUNNING  MTU:65536  Metric:1
          RX packets:6 errors:0 dropped:0 overruns:0 frame:0
          TX packets:6 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:0
          RX bytes:3252 (3.1 KiB)  TX bytes:3252 (3.1 KiB)

		  

**6. Show forward and reverse host lookups using getent and nslookup**

[hduser@SEBCxinyi ~]$ getent hosts
127.0.0.1       localhost localhost.localdomain localhost4 localhost4.localdomain4
127.0.0.1       localhost localhost.localdomain localhost6 localhost6.localdomain6
172.16.7.7      SEBCxinyi
172.16.7.10     SEBCxinyi-01
172.16.7.11     SEBCxinyi-02
172.16.7.12     SEBCxinyi-03
172.16.7.13     SEBCxinyi-04

[hduser@SEBCxinyi ~]$ ping -c 3 SEBCxinyi-01
PING SEBCxinyi-01 (172.16.7.10) 56(84) bytes of data.
64 bytes from SEBCxinyi-01 (172.16.7.10): icmp_seq=1 ttl=64 time=1.54 ms
64 bytes from SEBCxinyi-01 (172.16.7.10): icmp_seq=2 ttl=64 time=0.442 ms
64 bytes from SEBCxinyi-01 (172.16.7.10): icmp_seq=3 ttl=64 time=0.466 ms

--- SEBCxinyi-01 ping statistics ---
3 packets transmitted, 3 received, 0% packet loss, time 2002ms
rtt min/avg/max/mdev = 0.442/0.818/1.548/0.516 ms

		  

**7. Verify the nscd service is running**

[hduser@SEBCxinyi ~]$ sudo service nscd status
nscd (pid 6741) is running...
		 
		 

**8. Verify the ntpd service is running**

[hduser@SEBCxinyi ~]$ sudo service ntpd status
ntpd (pid  5420) is running...

[hduser@SEBCxinyi ~]$ ntpstat
synchronised to NTP server (202.156.0.34) at stratum 2
   time correct to within 3939 ms
   polling server every 64 s

   
