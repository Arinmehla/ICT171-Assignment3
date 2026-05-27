# Testing and Validation

These tests are done, to confirm that the server is working completely.

## Nginx running status test:
**sudo systemctl status nginx**

Result:

Active: active (running)

## Website File Test:
ls -l /var/www/html

This confirmed that the website files were stored in the correct Nginx web directory.


## HTTPS Website Test
curl -I https://arinmehla.info

**Result:**
HTTP/1.1 200 OK

This confirmed that the website is online and accessible through HTTPS.


## HTTP Redirect Test
curl -I http://arinmehla.info

Result:
HTTP/1.1 301 Moved Permanently
Location: https://arinmehla.info/
This confirmed that HTTP traffic redirected to HTTPS.


## Nginx Configuration Test
sudo nginx -t

This command is used to confirm that the Nginx configuration had no syntax errors.

## Automation Script Test:

I started with stopping the Nginx.
"sudo systemctl stop nginx"

After, I stopped Nginx my website stopped working while my Azure VM is still running. I started to recieve emails after every 5 minutes. This shows that my automation script is working correctly. After that, I restarted my website again.

"sudo systemctl start nginx"

To, confirm that my website started to work again.

"curl -I https://arinmehla.info"

The result is: HTTP/1.1 200 OK

