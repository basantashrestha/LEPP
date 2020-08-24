https://linuxhint.com/postgresql_docker/
Implements Nginx, PHP, PHP COMPOSER, POSTGRESQL AND PGADMIN   

Make following changes in /etc/hosts on the host system. Use DNS on real system.  
127.0.0.1       sample.localhost.localdomain            sample  


#Clone Repository  
git clone https://github.com/basantashrestha/LEMP.git  
cd LEPP
docker-compose up -d  


#Check on Browser  
http://sample.localhost.localdomain  
or  
http://sample.localhost.localdomain/info.php  


#To add virtual host. Make corresponding changes. Exmple is given below  
cp -r app/vhost-sample app/example.com  
cp config/nginx/vhost-sample.conf to config/nginx/example.com.conf  

##Access pgadmin Reference: https://linuxhint.com/postgresql_docker/ 
http://sample.localhost.localdomain:16543  
username:  test@gmail.com 
password: test123! ( As given in docker-compose.yml)    


##For SSL we need to work with real domain . The following video can be helpful   . 

https://www.youtube.com/watch?v=m9aa7xqX67c  

