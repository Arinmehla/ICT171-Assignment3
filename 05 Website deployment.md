# Website Deployment

After installing and starting Nginx, I deployed my website by editing the HTML default Nginx web directory with my file.

First, I moved into the Nginx web directory:

**cd /var/www/html**

Checked the files

**ls -l**

Edited the main nginx file with my content

**sudo nano index.html**

To load my new content properly need to restart the nginx

**sudo systemctl restart nginx**

Then, test the website with public IP address

**curl -I http://20.92.249.85**
