# ICT171 Assignment 3 

# Project Overview:
For my project, I created a cloud server using Microsoft Azure. I used an Azure student subscription, which initially provided me with some free credits. My server is created using infrastructure as a service (IAAS) because I manually configured everything myself I had direct SSH access to my virtual machine. I configured my network ports. I assigned everything myself, like RAM, ROM, and CPUs. I configured the network ports, and I installed Nginx, created an HTML website, used Namecheap to buy my domain name, and configured HTTPS and SSL. My website is about a classic cars showcase. It is a normal HTML website that displays information about some selected classic cars.

## I used Infrastructure as a Service (IAAS) because I wanted to create and manage my own cloud virtual machine instead of using a prebuilt platform with limited resources.
o	I created the Azure virtual machine.

o	I connected my VM to the server using SSH.

o	I configured network ports.

o	I installed and configured Nginx.

o	I uploaded stuff to my website.

o	I connected a custom domain name to my website.

o	I configured HTTPS and SSL.

## Port	Service	Purpose

22	SSH	         	 allows remote command-line access to the server

80	HTTP		allows normal website traffic

443	HTTPS		allows secure website traffic

**These ports were required for managing my server an allows users to access my website through a browser.**

Then I created an automated script that lets me know whether my website is running or it's down. If it's down, then it will send me an email. My script checks my website every 5 minutes.
