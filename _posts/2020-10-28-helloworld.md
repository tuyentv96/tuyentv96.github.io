---
layout: post
title: Sample blog post
subtitle: Each post also has a subtitle
gh-repo: daattali/beautiful-jekyll
gh-badge: [star, fork, follow]
tags: [test]
comments: true
---

This is a demo post to show you how to write blog posts with markdown.  I strongly encourage you to [take 5 minutes to learn how to write in markdown](https://markdowntutorial.com/) - it'll teach you how to transform regular text into bold/italics/headings/tables/etc.

**Here is some bold text**

## Here is a secondary heading

Here's a useless table:

| Number | Next number | Previous number |
| :------ |:--- | :--- |
| Five | Six | Four |
| Ten | Eleven | Nine |
| Seven | Eight | Six |
| Two | Three | One |
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
