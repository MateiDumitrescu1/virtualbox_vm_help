# virtualbox_vm_help

### configure shared folders
add a shared folder, tick auto-mount when making it 
for debian 12: https://itslinuxfoss.com/install-virtualbox-guest-additions-debian-12/
Add yourself to the vboxsf group within the guest VM.
```bash
add a shared folder, tick auto-mount
```

### user is not in sudoers file


### setup ssh from host to guest: port forwarding 
in virtualbox, click on a vm -> settings -> network -> expand the "Advanced" menu -> port forwarding -> add a rule with "Host Port" = 2222, "Guest Port" = 22
then you can 
```bash
ssh -p 2222 username@localhost"
```
