# Problems I faced and their Fixes
## Problem 1: Azure Subscription Stopped
At one point, my Azure for Students subscription ran out of available free credit, which caused the website to stop running. I fixed the Azure subscription and starting the virtual machine again.

# Problem 2: Website timing out when using the public IP address in the beginning
In the beginning, I faced a problem while opening my website using my public IP address before purchasing my domain name. When I try to open my website through the IP address, it does not load, and the request times out. After digging through, I realised that I had not assigned the needed ports to my server yet. So, I assigned port 80, which is for HTTP, and later I assigned HTTPS to run the website on my domain name.

# Problem 3: Website works on the domain name but not directly on the IP address
In the end, I noticed that my website is working properly when I use my domain name, but it is not loading properly when I use my public IP address. This is happening because I configured my nginx and HTTPS for my domain name. So now my website is configured to respond to my domain name. That's why it is not working properly on my public IP address.

## Problem 4: Bash Script Syntax Error
While creating the Bash script, I received this error:
syntax error: unexpected end of file
This happened because the Bash if statement was not closed correctly. I fixed the issue by adding:
fi
at the end of the if statement.
