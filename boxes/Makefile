boxes all: windows_2016_docker_virtualbox.box

windows_2016_docker_virtualbox.box : windows_2016_docker.json
	packer build --only=virtualbox-iso $<
