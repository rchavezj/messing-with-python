# Python DevOps

### This repo will contain any references to deploy API's with Python (Django/Flask) using the following: Vagrant, Docker containers, or AWS (Lambda, Gateway, EC2, Serverless). 


![alt text](https://github.com/rchavezj/Pyhon_DevOps/blob/master/Images/Python_DevOps.PNG)


# Contents: 
|                        |                                          |
| ---------------------- | ---------------------------------------- |
| 1. [Setup Environment Commands](#Setup)                         | 2. [Profile API](#Profile_API) |


### [Setup](#)
Make sure you have the following commands setup on ur API project </br>
(1) vagrant init ubuntu/bionic64: Create a configuration file Vagrantfile with server support (ubuntu/bionic64). Somtimes you will need to edit the Vagrantfile in order to setup step (2) properly.   </br>
(2) vagrant up: Download the base image specified inside VagrantFile configuration then start a virtual machine setup with ubuntu server.  </br>
(3) vagrant ssh: Connect to vagrant server as a 'guest' which is why we use the ssh flag on our command. Ubuntu commands are not the same as windows or mac. 
![alt text](https://github.com/rchavezj/Pyhon_DevOps/blob/master/Images/vagrantSSH.png)
(4) exit: If you ever wish to exit the development server and back to you're local machine. 

### [Vagrant Tips](#)
Make sure you enter the vagrant environment with the following commands
(1) Development repo is under the folder /vagrant


### [Profile_API](#)
[(Return back to Contents)](#Contents)
<img src="#" width="700">
