# Project-5
 CLIENT/SERVER ARCHITECTURE USING A MYSQL RELATIONAL DATABASE MANAGEMENT SYSTEM

Client-Server architecture describe the relationship between two or more connectecd computers sharing data across the network. In a client-server architecture, the client is the computer that requests for data, while the one that processes the request is known as the server.

To demonstrate, following the instructions below carefully.

1. Create and configure two Linux-based virtual servers (EC2 instances in AWS).

2. Name one instance Mysql-server the other Mysql-client

3. On mysql server Linux Server install MySQL Server using the following command.

`sudo apt install mysql-server -y`

4. On mysql client Linux Server install MySQL Client software.

`sudo apt install mysql-client -y`

5. Open port 3306 on Mysql-server allow for connection. You can do this by editing the Inbound Rules on the AWS Ec2 instance. Both server can communicate using private IPs since they belong to the same subnet

6. Change bind-address on Mysql-server to allow for connection from any IP address. Set the bind-address to 0.0.0.0 using the command below:

`sudo vi /etc/mysql/mysql.conf.d/mysqld.cnf`

7. From mysql client Linux Server connect remotely to mysql server Database Engine without using SSH. You must use the mysql utility to perform this action.

8. Check that you have successfully connected to a remote MySQL server and can perform SQL queries. You should something similar to the screenshot below:

![NGINX Status](./Images-5/image-5.1.jpg)
