# Mac OS X

## All OSX image are base on image from [sickcodes](https://sick.codes)
For more information : https://github.com/sickcodes/Docker-OSX

## Login information
- user = *user*
- password = *alpine*

## Many images are available
- [Base on Catalina](./catalina-images.md)
- [Base on Big Sur](./bigsur-images.md)

## Useful command
### Start a new docker with desktop
`docker run -it --name docker_macosx --device /dev/kvm -p 50922:10022 -v /tmp/.X11-unix:/tmp/.X11-unix -e "DISPLAY=${DISPLAY:-:0.0}" mickjol/macos-bigsur:base`

### Restart the last running image
`docker start -ai docker_macosx`

### Extract KVM image from container
- `docker cp docker_macosx:/home/arch/OSX-KVM/mac_hdd_ng.img .`

### Compressed KVM image before building docker image
- `qemu-img convert -O qcow2 mac_hdd_ng.img deduped.img`
- `qemu-img convert -c -O qcow2 deduped.img compressed.img`
