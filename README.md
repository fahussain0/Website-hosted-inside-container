# Docker Website hosting inside a container

	1. Install docker on ubuntu via CLI
	
	For Reference: 
	
	https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository
	
	2. Verify docker installation using 
	
	$ sudo docker run hello-world

	3. Run container with following settings

	$ docker run -it -p 80:80 --name nginx_container ubuntu:20.04

>	Note: To peek into running container use this cmd

	$ docker exec -it container_NameOR_ID /bin/bash

	After getting inside running container start creating layers over the running container.
