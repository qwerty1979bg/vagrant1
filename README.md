# A Vagrantfile for the first 5 vagrant tasks:

Usage:
```
vagrant up
vagrant ssh
vagrant destroy
```

- [x] "Use your own box from Vagrant Cloud"
- [x] "Change hostname to 'bananas3'"
- [x] "Script to install nginx"
- [x] "Set ip to 192.168.56.56"
- [x] "Set ip to 192.168.56.56"
- [x] "set port_forward 8080 - 80"

### Obsolete. Preserved for posterity:

Usage:
```shell
for name in (own_box, bananas3, nginx, ip, fwd) do
  vagrant up <name>
  vagrant ssh <name>
  *play around*
done

vagrant destroy /./
```
