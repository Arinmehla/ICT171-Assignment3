# Domain Name:
After my website is working through the Azure public IP address, I purchased my custom domain name from Namecheap.
## My domain name is “arinmehla.info”
I configured my domain name to point to the Azure virtual machine public IP address:
**20.92.249.85**
After that, I tested my domain with the command:
**ping arinmehla.info**
It confirmed to me that the domain resolved to the correct public IP address. The website was successfully configured with HTTPS. I used curl to test my website.

# HTTPS/SSL Configuration:

The HTTPS website was tested using:

**curl -I https://arinmehla.info**

The successful output was:

**HTTP/1.1 200 OK**

Server: nginx/1.24.0 (Ubuntu)
Content-Type: text/html

**This confirms that the website is accessible through HTTPS.**


