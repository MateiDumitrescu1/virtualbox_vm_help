# virtualbox_vm_help

### configure shared folders
for debian 12: https://itslinuxfoss.com/install-virtualbox-guest-additions-debian-12/


### user is not in sudoers file


### setup ssh from host to guest: port forwarding 
in virtualbox, click on a vm -> settings -> network -> expand the "Advanced" menu -> port forwarding -> add a rule with "Host Port" = 2222, "Guest Port" = 22
then you can "ssh -p 2222 username@localhost"
