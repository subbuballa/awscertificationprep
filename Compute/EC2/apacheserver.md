### Installing an Apache server and rendering data

1. Get to elevated permissions, so that you can run all the commands with out any issues.   

    > What is the command to elevate permissions on the EC2 machine?  
    ***sudo su***

2. Update to the latest, forces to update itself  

    > What is the command to update EC2 instance  
    yum update -y

3. How to install httpd - Apache server?  

    > What is the command to install Apache server?  
    ***yum install -y httpd.x86_64***  
    How to start the service?  
    ***systemctl httpd.service***  
    How to keep apache server running after reboots?  
    ***systemctl enable httpd.service ***

4. How to render http traffic from EC2 instance?  
Once apache is installed, it servers it traffic through port 80. So inorder to render the pages, open up port 80 in the inbound rules for the EC2 instance.  

5. What is the default location from where apache server renders its content  
    > /var/www/html/index.html
