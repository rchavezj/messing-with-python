# Python DevOps

### This repo will contain any references to deploy APIs with Python (FastAPI/Django/Flask) using the following: Vagrant, Docker containers, or AWS (Lambda, Gateway, Serverless, torchserve via PyTorch).

![alt text](https://github.com/rchavezj/Pyhon_DevOps/blob/master/Images/Python_DevOps.PNG)
![alt text](https://github.com/rchavezj/Pyhon_DevOps/blob/master/Images/torchServe.gif)
![alt text](https://github.com/rchavezj/Pyhon_DevOps/blob/master/Images/microservices.png)

# Contents:

|                                         |                                |
| --------------------------------------- | ------------------------------ |
| 1. [Setup Environment Commands](#Setup) | 2. [Profile API (Django)](#Profile_API) |
| 3. [Hello world (FastAPI)](#Setup) | 4. [PyTorch Image model (Flask)](#) |

### [Vagrant Setup](#)

Make sure you have the following commands setup on ur API project </br>
(1) Create a configuration file Vagrantfile with server support (ubuntu/bionic64). Somtimes you will need to edit the Vagrantfile in order to setup step (2) properly. 
```console 
vagrant init ubuntu/bionic64
``` 
(2) Download the base image specified inside VagrantFile configuration then start a virtual machine setup with ubuntu server.
```console
vagrant up 
``` 

(3) Connect to vagrant server as a 'guest' which is why we use the ssh flag on our command. Ubuntu commands are not the same as windows or mac. 
```console 
vagrant ssh
```

![alt text](https://github.com/rchavezj/Pyhon_DevOps/blob/master/Images/vagrantSSH.png) </br>
(4) exit --> If you ever wish to exit the development server and back to you're local machine.

### [Vagrant Tips](#)

(0) Make sure you change directories to the path '/vagrant' inside of the virtua ubuntu. </br>
(1) Development repo is under the folder /vagrant using the command 'cd /vagrant' </br>
(2) Create python environment onto server.
```console 
python -m venv ~/env
```

(3) Activate virtual env  
```console 
source ~/env/bin/activate
```
(4) Deactivate virtual environment. 
```console 
deactivate
```

### Dependency (install inside vagrant env activated)
```console 
pip install -r requirements.txt </br>
```
### Django Admin Setip

(1) the script (django-admin.py) is passed in and the argument "startproject" is
a flag to start a new project (profiles_project). the "." is an optional argument 
to place the folder on the root of invoked command.
```console 
django-admin.py startproject profiles_project .  
```

is passed in and the argument "startproject" is </br>
a flag to start a new project (profiles_project). </br>
the "." is an optional argument to place the folder on the root of invoked command. </br>
(2) Start a new django api project using manage.py 
```console 
python manage.py startapp [name]
```
(3) Inside of settings.py, repo inside of django api project from step (2), add in the following apps </br>
![alt text](https://github.com/rchavezj/Pyhon_DevOps/blob/master/Images/settings.png)
(4) On the browser type in 'http://127.0.0.1:8000/' to view ur code on the server. Django place holder (img of a rocket) is set to default.
```console 
python manage.py runserver 0.0.0.0:8000
```
(4a)  If running the local host ends up in an infinite loop. 
```console 
python manage.py runserver --noreload 0.0.0.0:8000 
```

### Django Migration setup
These two can create an init file (0001_initial.py) 
```console
python manage.py migrate
python manage.py makemigrations [name: profiles_api] 
```

### Django Create superuser
```console
python manage.py createsuperuser 
```

### [Profile_API](#)

[(Return back to Contents)](#Contents)
<img src="#" width="700">
