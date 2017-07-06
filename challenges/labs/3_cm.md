Listing the directories within the /user
```
[ec2-user@ip-172-31-15-71 ~]$ HADOOP_USER_NAME=hdfs hadoop fs -ls /user
Found 5 items
drwxrwxrwx   - mapred   hadoop              0 2017-07-06 11:56 /user/history
drwxrwxr-t   - hive     hive                0 2017-07-06 11:57 /user/hive
drwxrwxr-x   - hue      hue                 0 2017-07-06 11:58 /user/hue
drwxr-xr-x   - userName supergroup          0 2017-07-06 12:15 /user/neymar
drwxrwxr-x   - oozie    oozie               0 2017-07-06 11:58 /user/oozie
[ec2-user@ip-172-31-15-71 ~]$ ^C
[ec2-user@ip-172-31-15-71 ~]$ 




