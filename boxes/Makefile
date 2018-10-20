boxes all: windows_2016_docker_virtualbox.box

windows_2016_docker_virtualbox.box : ../packer-windows/windows_2016_docker.json
	(cd ../packer-windows; packer build -only=virtualbox-iso -var disk_size=153600 $<; mv "$@" ../boxes)
