# MEAN-Application
MYSQL, EXPRESS, ANGULAR, NODEJS

For MYSQL setup 
**********************************************************
mysql> create database bankdb;

mysql> use bankdb;

mysql> create table agents(agentId double PRIMARY KEY AUTO_INCREMENT,agentName v
archar(10),agentPassword varchar(15));

mysql> alter table agents AUTO_INCREMENT=15000;

mysql> create table customers(accountNumber double PRIMARY KEY AUTO_INCREMENT,fi
rstName varchar(15),lastName varchar(15),fatherName varchar(15),motherName varch
ar(15),age int,gender varchar(10),mobileNumber double,amount double,address varc
har(25),dateOfBirth DATE,type varchar(10));

mysql> alter table customers AUTO_INCREMENT=100000;

mysql> create table customerAccount(accountNumber double PRIMARY KEY,firstName
archar(15),lastName varchar(15),password varchar(15));


******************************************************************************
if this error occurs

Error: ER_NOT_SUPPORTED_AUTH_MODE: Client does not support authentication protocol requested by server; consider upgrading MySQL client

then run this commands

mysql> ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'r
oot';

mysql> flush privileges;

********************************************************************************************


