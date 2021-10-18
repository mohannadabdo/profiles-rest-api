#PROFILES REST API

Profiles REST API course code.

Used Vagarant as local development server to run and test api as we build it.

**$ vagrant init ubuntu/bionic64**

We can Customize our vagrant file.

**$ vagrant up**

Used to download the base image in vagrant file and use virtual box to create

**$ vagrant ssh**

will connect to vagrant box

so because the development server is a virtual machine on our computer by

default the file system is not synchronized that means that all of the

files on our development server are different from the files on our local

machine

vagrant works by creating a synchronized directory on our vagrant

server that updates itself with all of the files in our local project every

time we make changes


**$ cd /vagrant**

the vagrant directory on our server is synchronized with everything in our project folder
