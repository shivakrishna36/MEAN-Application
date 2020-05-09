# MEAN-Application
MYSQL, EXPRESS, ANGULAR, NODEJS

-------------------------------------------------------------------------------------------------------------------------------------

prerequisite
***************************************
Make sure Node Js is installed version is 12 or above
Make sure angularCli is installed version 8 or above
Mysql is installed

-------------------------------------------------------------------------------------------------------------------------------------

For Angular setup
*******************************************************
1. After the zip file is downloaded Extract and open bankApplication folder.
2. From that current folder where src is present open cmd from there.
3. Run command as 'npm install'
4. Next, Run command 'ng serve'

-------------------------------------------------------------------------------------------------------------------------------------

For Node js setup
*************************************************************
1. After the zip file is downloaded Extract and open bankapp folder.
2. From that current folder where index.js is present open cmd from there.
3. Run command as 'npm install'
4.Next, run command 'node index.js'

-------------------------------------------------------------------------------------------------------------------------------------

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


