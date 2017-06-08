# etherpad-docker
Docker for etherpad with mysql

````
$> cd etherpad-docker
$> docker-compose up
````

### migrate data into mysql container:
````
$> sudo docker exec -it <mysql_contianer_id> /bin/bash
$> mysql -u root -p etherpad < /var/lib/etherpad_data/etherpad.sql
````