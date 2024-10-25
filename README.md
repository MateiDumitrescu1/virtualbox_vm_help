# virtualbox_vm_help

### configure shared folders
add a shared folder, tick auto-mount when making it 

install virtual box guest additions 

for debian 12: https://itslinuxfoss.com/install-virtualbox-guest-additions-debian-12/

reboot
```bash
sudo reboot
```
Add yourself to the vboxsf group within the guest VM.
then reboot
```bash
sudo adduser $USER vboxsf
sudo reboot
```

Check out the shared folder on the Guest!! It will be called sf_something
```bash
cd /media
ls -a
```
### user is not in sudoers file


### setup ssh from host to guest: port forwarding 
in virtualbox, click on a vm -> settings -> network -> expand the "Advanced" menu -> port forwarding -> add a rule with "Host Port" = 2222, "Guest Port" = 22
then you can 
```bash
ssh -p 2222 username@localhost"
```


### to use docker without sudo -> create a user group called docker, add current user to it 
```bash
sudo groupadd docker
sudo usermod -aG docker $USER
```

### assign static ip to vm in virtualbox
