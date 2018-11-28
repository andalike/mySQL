# mySQL
sudo apt-get update
sudo apt-get install mysql-server
mysql_secure_installation
    
## Removing MYSQL
sudo apt-get purge mysql-server mysql-client mysql-common mysql-server-core-* mysql-client-core-*
sudo rm -rf /etc/mysql /var/lib/mysql
sudo apt-get autoremove
sudo apt-get autoclean
    
    
    
