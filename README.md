# nodejs-in-windows-docker
Tools for nodejs to be less painful in windows containers for docker

## Pre-reqs
* A machine with virtualbox
* Docker-machine
* Docker
* Packer


## Build/Setup
### Create Vagrant Box

``` bash
make boxes && make install_boxes
```

## Incompatibilities
* Ubuntu's Docker Snap
  * docker-machine cannot find ~/.docker/machine
