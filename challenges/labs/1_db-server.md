# DB Server node
```
[ec2-user@ip-172-31-15-71 ~]$ hostname -f
ip-172-31-15-71.eu-central-1.compute.internal
```

# Command to display DB server's version
 ```
[ec2-user@ip-172-31-15-71 ~]$ mysql --version
mysql  Ver 14.14 Distrib 5.5.56, for Linux (x86_64) using readline 5.1

```
# List of all the databases
```
mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| amon               |
| hive               |
| hue                |
| mysql              |
| nav                |
| navms              |
| oozie              |
| performance_schema |
| rman               |
| scm                |
| sentry             |
+--------------------+
12 rows in set (0.00 sec)

mysql> 

