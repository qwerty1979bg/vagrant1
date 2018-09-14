# A Vagrantfile for the first 4 vagrant tasks:

Usage:
```
vagrant up
vagrant ssh
vagrant destroy
```

###For the museum:

- [x] "Use your own box from Vagrant Cloud"
- [x] "Change hostname to 'bananas3'"
- [x] "Script to install nginx"
- [x] "Set ip to 192.168.56.56"

Usage:
```shell
for name in (own_box, bananas3, nginx, ip) do
vagrant up <name>
vagrant ssh <name>
*play around*
done
vagrant destroy /./
```
