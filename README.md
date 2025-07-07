# ec_control

Intel方案
参考资料
https://eci.intel.com/embodied-sdk-docs/content/installation_setup/installation/rt_linux.html
https://eci.intel.com/embodied-sdk-docs/content/developer_tools_tutorials/oneapi.html


开机后，启动主站

intel@intel:~$ sudo /etc/init.d/ethercat restart
Shutting down EtherCAT master 1.6.0 /etc/init.d/ethercat: 228: echo: echo: I/O error
done
Starting EtherCAT master 1.6.0  done
intel@intel:~$
intel@intel:~$ sudo ethercat master
Master0
Phase: Idle
Active: no
Slaves: 1
Ethernet devices:
Main: 68:ed:a4:44:c6:6c (attached)
Link: UP
Tx frames:   4682
Tx bytes:    370072
Rx frames:   4681
Rx bytes:    370012
Tx errors:   0
Tx frame rate [1/s]:    245    367     74
Tx rate [KByte/s]:     14.4   29.3    5.8
Rx frame rate [1/s]:    245    367     74
Rx rate [KByte/s]:     14.4   29.3    5.8
Common:
Tx frames:   4682
Tx bytes:    370072
Rx frames:   4681
Rx bytes:    370012
Lost frames: 0
Tx frame rate [1/s]:    245    367     74
Tx rate [KByte/s]:     14.4   29.3    5.8
Rx frame rate [1/s]:    245    367     74
Rx rate [KByte/s]:     14.4   29.3    5.8
Loss rate [1/s]:          0      0      0
Frame loss [%]:         0.0    0.0    0.0
Distributed clocks:
Reference clock:   Slave 0
DC reference time: 0
Application time:  0
2000-01-01 00:00:00.000000000
intel@intel:~$
intel@intel:~$ sudo ethercat slaves
0  0:0  PREOP  +  SSC-Device
intel@intel:~$ 
