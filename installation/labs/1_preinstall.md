vm.swappiness = 1
/dev/sdc1 on /data01 type ext3 (rw,relatime,seclabel,data=ordered)

/* ----------------------------------------------------------------------------- */

cat /proc/sys/vm/nr_hugepages
0

/* ----------------------------------------------------------------------------- */

ifconfig -a
eth0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 10.5.0.5  netmask 255.255.255.128  broadcast 10.5.0.127
        inet6 fe80::20d:3aff:fea1:c871  prefixlen 64  scopeid 0x20<link>
        ether 00:0d:3a:a1:c8:71  txqueuelen 1000  (Ethernet)
        RX packets 8058  bytes 3749746 (3.5 MiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 8956  bytes 1317118 (1.2 MiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1  (Local Loopback)
        RX packets 64  bytes 5568 (5.4 KiB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 64  bytes 5568 (5.4 KiB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

/* ----------------------------------------------------------------------------- */

nslookup aria-cloudera02
Server:		168.63.129.16
Address:	168.63.129.16#53

Name:	aria-cloudera02.khepdbovhx5upmbxp4bqq1hzyc.ix.internal.cloudapp.net
Address: 10.5.0.5
