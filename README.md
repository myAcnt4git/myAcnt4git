# myAcnt4git
1. create an ubuntu container on Windows 10
	a. under windows prompt
           
	   docker pull dorowu/ubuntu-desktop-lxde-vnc:bionic
	   docker run --name vbvnc -p 6080:80 -p 5900:5900 dorowu/ubuntu-desktop-lxde-vnc:bionic

2. access ubuntu
	visit http://127.0.0.1:6080/#/	/* which runs  noVNC more limited java vnc client */

3. get into ubuntu terminal
        through the GUI, go to [Appliction] -> [System Tools] -> [LXterminal]
        a terminal window will be open with root user

4. provision ubuntu
	a. first install git
	b. configure user's account
	c. login to my repository
	d. edit README.md
	e. git commit and git push

5. provision ubuntu further
	a. install docker so we can play docker within a docker
	b. edit a docker file for centos-6
	c. generate a centos-6 container to build open source packages
		. tensorflow-2.5
		. protobuf 3.7.0
		. bazel 3.73.0
		. gcc 3.7.0
