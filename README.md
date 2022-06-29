# mySQL
sudo apt-get update <br />
sudo apt-get install mysql-server <br />
mysql_secure_installation <br />
    
## Removing MYSQL
sudo apt-get purge mysql-server mysql-client mysql-common mysql-server-core-* mysql-client-core-* <br />
sudo rm -rf /etc/mysql /var/lib/mysql <br />
sudo apt-get autoremove <br />
sudo apt-get autoclean <br />
    
    
## Connect to Database
mysql -u root -p 

## Creating Database BackUp
mysqldump -u root -p --all-databases > all_db_backup.sql

## Restoring Database BackUp
sudo mysql -u root -p menagerie < all_db_backup1.sql

## MYSQL Using Docker
sudo docker run --name=mysql1 -d mysql/mysql-server:5.7

## Create a MySQL Instance
Create a MySQL instance using AMI for version 5.7

## Connecting to External Machine
 mysql -u admin -p -h database-1.someaddress.ap-south-1.rds.amazonaws.com -P 3306

