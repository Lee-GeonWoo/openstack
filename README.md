# Install Openstack (wallaby ver.)

It should be connected by 2 LAN lines.
```
$ ifconfig
```
After checking the interface, copy the INTERFACE_ID that inet is not set (ex. eno2 or enx~~)
```
$ source openstack_installation.sh ${INTERFACE_ID}
```
Set Openstack Dashboard Password
