---
layout: post
title: Installing Nginx On Ubuntu
tags: [nginx,proxy]
comments: true
---

## Step 1 - Installing nginx
Because Nginx is available in Ubuntu’s default repositories, it is possible to install it from these repositories using the `apt` packaging system.
~~~
sudo apt update
sudo apt install nginx
~~~

After accepting the procedure,  `apt`  will install Nginx and any required dependencies to your server.
## Step 2 – Adjusting the Firewall
Before testing Nginx, the firewall software needs to be adjusted to allow access to the service. Nginx registers itself as a service with  `ufw`  upon installation, making it straightforward to allow Nginx access.
~~~
sudo ufw allow 'Nginx HTTP'
~~~
## Step 3 – Checking your Web Server
We can check with the  `systemd`  init system to make sure the service is running by typing:
```
systemctl status nginx
```
## Step 4 – Managing the Nginx Process
To enable the service to start up at boot, you can type:
```
sudo systemctl enable nginx
```
To start the service, you can type:
```
sudo systemctl start nginx
```
