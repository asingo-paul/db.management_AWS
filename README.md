# db.management_AWS
I am currently managing a database on an ec2 instance for an application on two different availability zones
## installation of mysql on ubuntu EC2 intance.

what you would want to do after creating an ec2 instance is to try and update the system to get the latest update
-     sudo apt update && sudo apt upgrade -y

this command below installs mysql and also passes a security script too
-     sudo apt install mysql-server
      sudo mysql_secure_installation
![Screenshot 2025-07-09 172815](https://github.com/user-attachments/assets/66fdbc65-37b3-4a9a-95fe-15e989d4c66b)


  
-     mysql --version
-     sudo systemctl start mysql  # Start the service do
      systemctl stop mysql   # Stop the service
      sudo systemctl restart mysql # Restart the service
## next on
