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

	4. Update ubuntu container and Install nginx inside container

		# apt-get update | apt-get install nginx -y

	5. Now verify nginx is running or not

		$ service nginx enable
		$ service nginx start
		$ service nginx status

	6. Now install vim to edit text files inside container

		$ apt-get install vim

	7. Now we will install curl to test website inside container

		$ apt-get install curl

	8. Now follow Points 9 and 10 from this README.md of my other wonderful project for website deployment:

	https://github.com/fahussain0/nginx_deployment/blob/main/README.md

