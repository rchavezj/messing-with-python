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
(3) vagrant ssh: Connect to vagrant server as a 'guest' which is why we use the ssh flag on our command. Ubuntu commands are not the same as windows or mac. </br>
![alt text](https://github.com/rchavezj/Pyhon_DevOps/blob/master/Images/vagrantSSH.png)
(4) exit: If you ever wish to exit the development server and back to you're local machine. 


### [Vagrant Tips](#)
Make sure you enter the vagrant environment with the following commands </br>
(1) Development repo is under the fothe base image specified inside VagrantFile configuration then start a virtual machine setup with ubuntu server.  </br>
(3) vagrant ssh: Connect to vagrant server as a 'guest' which is why we use the ssh flag on our command. Ubuntu commands are not the same as windows or mac. </br>
![alt text](https://github.com/rchavezj/Pyhon_DevOps/blob/master/Images/vagrantSSH.png) </br>
(4) exit: If you ever wish to exit the development server and back to you're local machine. 



### [Vagrant Tips](#)
Make sure you enter the vagrant environment with the following commands </br>
(1) Development repo is under the folder /vagrant </br>
(2) python -m venv ~/env: Create python environment onto server. </br> 
(3) source ~/env/bin/activate: Activate virtual env </br>
(4) deactivate: Deactivate virtual environment.
</br> 

### Dependency (install inside vagrant env activated)
pip install -r requirements.txt </br>

### Django Admin Setip
(1) django-admin.py startproject profiles_project . </br>
the script (django-admin.py) is passed in and the argument </br>
"startproject" is a flag to start a new project (profiles_project). </br>
the "." is an optional argument to place the folder on the root of invoked command.  </br>
(2) python manage.py startapp [name]: Start a new django api project using manage.py</br>
(3) Inside of settings.py, repo inside of django api project from step (2), add in the following apps </br>
![alt text](https://github.com/rchavezj/Pyhon_DevOps/blob/master/Images/settings.png)

### [Profile_API](#)
[(Return back to Contents)](#Contents)
<img src="#" width="700">
