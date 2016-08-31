Installation Docker
===================
Installing docker  on Ubuntu::

        sudo apt-get update
        sudo apt-get install docker.io
Installing docker on centos::
	sudo yum update
Add the yum repo::
	sudo tee /etc/yum.repos.d/docker.repo <<-'EOF'
	[dockerrepo]
	name=Docker Repository
	baseurl=https://yum.dockerproject.org/repo/main/centos/7/
	enabled=1
	gpgcheck=1
	gpgkey=https://yum.dockerproject.org/gpg
	EOF
Install the Docker package::
	sudo yum install docker-engine
Start the Docker daemon::
	sudo service docker start
