# db.management_AWS
I am currently managing a database on an ec2 instance for an application on two different availability zones
## Installation of mysql on ubuntu EC2 intance.

What you would want to do after creating an ec2 instance is to try and update the system to get the latest update.
-     sudo apt update && sudo apt upgrade -y

This command below installs mysql and also passes a security script too.
this will allow you to perform these
- Set a root password
- Remove anonymous users
- Disallow remote root login
- Remove test databases
- Reload privilege tables
-     sudo apt install mysql-server
      sudo mysql_secure_installation
![Screenshot 2025-07-09 172815](https://github.com/user-attachments/assets/66fdbc65-37b3-4a9a-95fe-15e989d4c66b)


This just helps you confirm that mysql is installed and what version are you using at the point in time.
-     mysql --version
  ![Screenshot 2025-07-09 172941](https://github.com/user-attachments/assets/37875929-d96b-4a39-9705-1dd662b1708f)

## MySQL Service Management
In case MySQL is not running or encounters issues, manage the service using the following commands:
-     sudo systemctl start mysql  # Start the service do
      systemctl stop mysql   # Stop the service
      sudo systemctl restart mysql # Restart the service
### Troubleshooting Tip:
If MySQL fails to start, check the status or logs:
-      sudo systemctl status mysql
       sudo journalctl -xe
### Monitor MySQL Server Performance
Use the built-in MySQL tool
-      mysqladmin -u root -p processlist
       mysqladmin -u root -p status


