PACKER_CACHE_DIR ?= $(HOME)/packer_cache
export PACKER_CACHE_DIR

boxes all: windows_2016_docker_virtualbox.box

windows_2016_docker_virtualbox.box : ../packer-windows/windows_2016_docker.json
	echo $$PACKER_CACHE_DIR
	(cd ../packer-windows; packer build -only=virtualbox-iso -var disk_size=153600 $<; mv "$@" ../boxes)
