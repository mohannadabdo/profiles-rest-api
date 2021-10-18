# PROFILES REST API

Profiles REST API course code and notes.
# Vagrant Installation
Used Vagarant as local development server to run and test api as we build it.

**$ vagrant init ubuntu/bionic64**

We can Customize our vagrant file.

**$ vagrant up**

Used to download the base image in vagrant file and use virtual box to create

**$ vagrant ssh**

will connect to vagrant box. So because the development server is a virtual machine on our computer by default the file system is not synchronized that means that all of the files on our development server are different from the files on our local machine vagrant works by creating a synchronized directory on our vagrant server that updates itself with all of the files in our local project every time we make changes

**$ cd /vagrant**

the vagrant directory on our server is synchronized with everything in our project folder


# Create Python VIRtual environment

1) **$ vagrant ssh**

2) **$ cd /vagrant**

3) **$ python -m menv ~/env**

Creates a new file in vagrant server home directory /env and creates the python env there.

4) Activate python virtual environment

**$ source ~/env/bin/activate**

To Deactivate the python virtual environment
**$ Deactivate**

# Install required python packages
1) Create **requirments.txt**
2) **django==2.2**
3) **djangorestframework==3.9.2**
4) **$ vagrant ssh**
5) **$ cd /vagrant**
6) **source ~/env/bin/activate**
7) **pip install -r requirments.txt**

# Create django project and app
In the python virtual env:

1)  **django-admin.py startproject profiles_project .**
it calls the Django admin dot py script it passes in and the arguments start project to say that we want to start a new project and it specifies the name of the project so our project is going to be called the profiles underscore project and then the location that we want to create the project.
2)  **python manage.py startapp profiles_api**
Create application **profiles_api** in project **profiles_project**

# Enable Django application
1)navigate to profiles_project directory
2)navigate to **settings.py**
3)Add the following under **INSTALLED_APPS**:
**'rest_framework',  'rest_framework_authtoken', 'profiles_api',**

# test django application
1) 
