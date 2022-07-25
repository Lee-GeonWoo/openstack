# Install Openstack (wallaby ver.)

## Install Openstack
It should be connected by 2 LAN lines.
```
$ ifconfig
```

After checking the interface, copy the INTERFACE_ID that inet is not set (ex. eno2 or enx~~)
```
$ chmod +x openstack_installation.sh
$ source openstack_installation.sh ${INTERFACE_ID}
```

Set Openstack Dashboard Password



## Uninstall Openstack
```
$ sudo su - stack
$ cd devstack
$ ./unstack.sh
$ ./clean.sh
```

Delete stack user
```
$ sudo su -
$ rm -rf /opt/stack
$ rm -rf /usr/local/bin/
$ rm -rf /usr/local/lib/
$ userdel -rf stack
```
