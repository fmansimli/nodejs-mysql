# NodeJS ( TypeScript ) and MySQL

## Database creating and restoring with Docker

mypc >> docker run --name mysql-cont -p 3306:3306 -e MYSQL_ROOT_PASSWORD=12345 -d mysql

<br/>

mypc >> docker cp /path/sampledb.sql mysql-cont:/home/

<br/>

mypc >> docker exec -it mysql-cont bash

<hr/>

mysql>> source /home/sampledb.sql

<hr/>

mysql>> show databases;

<br/>

mysql>> exit
