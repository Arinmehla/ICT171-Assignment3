# SSL Certificate
After I connected my domain name to my Azure VM. I configured the SSL certificate that is needed to encrypt data travelling between a browser and a website.

## SSL Certificate Setup

My domain name is:

```text
arinmehla.info
```

My website was first working through HTTP:

```text
http://arinmehla.info
```

I also checked that the required ports were allowed in my Azure VM. Port 22 for SSH, port 80 for HTTP, and port 443 for HTTPS.

After confirming that the domain and web server were working, I used the Certbot Nginx on Linux.

I installed Certbot using snap:

```bash
sudo snap install --classic certbot
```

Then I linked the Certbot command so it could be used from the terminal:

```bash
sudo ln -s /snap/bin/certbot /usr/bin/certbot
```

After that, I requested the SSL certificate for my Nginx website:

```bash
sudo certbot --nginx
```

After the certificate was installed, I tested the Nginx configuration:

```bash
sudo nginx -t
```

Then I restarted Nginx:

```bash
sudo systemctl restart nginx
```

I tested the HTTPS version of my website using:

```bash
curl -I https://arinmehla.info
```
After completing this step, my website was accessible securely through:

```text
https://arinmehla.info
```

It was important because HTTPS makes the website more secure and also shows that the domain has a valid SSL certificate.
