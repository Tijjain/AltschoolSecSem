# AltschoolSecSem

#Webpage Public IP Address - 18.203.188.228

#Steps in setting up Webpage
1. Deployment of Virtual Machine (Cloud Instance) on AWS: This involved setting up an AWS account and creating a new ubuntu instance with the eligible free tier resources options in the eu-West1 region. A security group was then created and attached to the instance to allow required traffic (Inbound ssh, http and https) and Outbound All traffic)
2. Nginx Installation Ubuntu instance: ssh into to the ubuntu instance using the default ubuntu user and create a new admin user, also add user tp sudo group. To install nginx, sudo apt install nginx and once installed, check firewall settings sudo ufw app list. allow http
3. Build the index.wwwwhtml file 
4. Transfer html file to ubuntu server from local directory: Using scp -i path/to/pem path/to/file username@PublicDNS:~/file-path-in-EC2 transfer the html to the /var/www/html directory
5. Restart nginx service and refresh browser
