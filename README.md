# MacOSX
## All image are base on image from [sickcodes](https://sick.codes)
For more information : https://github.com/sickcodes/Docker-OSX

user = user, password = alpine

## Many image are available
[See all image](./IMAGES.md)

## Start an image with desktop
` docker run -it --device /dev/kvm -p 50922:10022 -v /tmp/.X11-unix:/tmp/.X11-unix -e "DISPLAY=${DISPLAY:-:0.0}" mickjol/macos-catalina:cordova`
