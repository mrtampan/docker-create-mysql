## tutorial membuat mysql didalam docker

docker container run -d --name mysqldb -p 3306:3306 -e MYSQL_ROOT_PASSWORD=password mysql:latest

docker exec -it mysqldb bash

mysql -u root -ppassword

show databases;

create database company;

drop database company;

use company;

create table team ( id int not null, name text, primary key (id) );

show tables; 

insert into team (id , name) values (1, 'Thetips4you');

insert into team (id , name) values (2, 'King');

insert into team (id , name) values (3, 'Queen');

select * from team;
