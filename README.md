# Ubuntu-netowrk-invalid
## Mount NetworkManager(network driver)
switch user to root `sudo su`
> in /etc/NetworkManager/NetworkManager.conf
```file
[ifupdown]
managed=True
```
## Remove NetworkManager state and restart service
```
service NetworkManager stop
rm /var/lib/NetworkManager/NetworkManager.state
service NetworkManager start
```
