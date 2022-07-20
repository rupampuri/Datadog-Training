# voda-datadog-11thjuly2022

<img src="plan.png">

## COde share link 

[clickhere](https://codeshare.io/N3dOEo)

### APM -- 

### SAMPle webapp 

<img src="sample.png">

### replace php8 to php7 

```
283  yum history list 
  284  yum history undo 10 
  285  yum history undo 11
  286  yum history undo 10 
```
###

```
 amazon-linux-extras disable  php8.0
 amazon-linux-extras enable php7.4
 yum clean metadata
 yum install php-cli php-pdo php-fpm php-json php-mysqlnd
 yum install php
 
```

### lets install Mairadb Db -- 

```
yum  install mariadb-server
[root@vaibhav-vm ~]# systemctl enable --now mariadb 
Created symlink from /etc/systemd/system/multi-user.target.wants/mariadb.service to /usr/lib/systemd/system/mariadb.service.
[root@vaibhav-vm ~]# systemctl status  mariadb 
● mariadb.service - MariaDB database server
   Loaded: loaded (/usr/lib/systemd/system/mariadb.service; enabled; vendor preset: disabled)
   Active: active (running) since Wed 2022-07-20 13:04:38 UTC; 18s ago
  Process: 29200 ExecStartP
  
```

### setup database configurations 

```
[root@vaibhav-vm ~]# mysql -u root -p
Enter password: 
Welcome to the MariaDB monitor.  Commands end with ; or \g.
Your MariaDB connection id is 10
Server version: 5.5.68-MariaDB MariaDB Server

Copyright (c) 2000, 2018, Oracle, MariaDB Corporation Ab and others.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

MariaDB [(none)]> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| performance_schema |
+--------------------+
3 rows in set (0.00 sec)

MariaDB [(none)]> create  database wordpress;
Query OK, 1 row affected (0.00 sec)

MariaDB [(none)]> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| mysql              |
| performance_schema |
| wordpress          |
+--------------------+
4 rows in set (0.00 sec)

MariaDB [(none)]> exit;
Bye

```


