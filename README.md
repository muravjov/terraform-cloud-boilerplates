# terraform-provider-libvirt boilerplates for popular cloud OSes

List of tested OSes:
```
centos7
centos8
debian10
opensuse15
ubuntu18.04
ubuntu20.04
```

## Preparation

1. Download [terraform](https://releases.hashicorp.com/terraform/) binary and save as `./terraform`
1. Download [terraform-provider-libvirt](https://github.com/dmacvicar/terraform-provider-libvirt/releases) binary and save as `./terraform-provider-libvirt`
1. Download the needed iso image and save in directory `./iso-images`
 
## Create/Destroy Cloud OS

For example, to install Debian 10:

```bash
./terraform apply debian10
virsh list
virsh console debian10
./terraform destroy debian10
virsh list --all
```

Login/Password: root/linux
