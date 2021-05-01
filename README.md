# MacOSX
## All image are base on image from [sickcodes](https://sick.codes)
For more information : https://github.com/sickcodes/Docker-OSX

user = user, password = alpine

## mickjol/macos-catalina:base
- Catalina 10.15.7

## mickjol/macos-catalina:code
- macos-catalina:base
- Visual Studio Code 1.55.2
- Xcode 12.2

## mickjol/macos-catalina:cordova
- macos-catalina:code
- NodeJs 14.16
- NPM 7.11
- Cordova 10.0

## Start an image with desktop
` docker run -it --device /dev/kvm -p 50922:10022 -v /tmp/.X11-unix:/tmp/.X11-unix -e "DISPLAY=${DISPLAY:-:0.0}" mickjol/macos-catalina:cordova`
