The first line of the Cloudera Manager server log

```[ec2-user@ip-172-31-15-71 ~]$ sudo head -1 /var/log/cloudera-scm-server/cloudera-scm-server.log
2017-07-06 11:34:21,041 INFO main:com.cloudera.server.cmf.Main: Starting SCM Server. JVM Args: [-Dlog4j.configuration=file:/etc/cloudera-scm-server/log4j.properties, -Dfile.encoding=UTF-8, -Dcmf.root.logger=INFO,LOGFILE, -Dcmf.log.dir=/var/log/cloudera-scm-server, -Dcmf.log.file=cloudera-scm-server.log, -Dcmf.jetty.threshhold=WARN, -Dcmf.schema.dir=/usr/share/cmf/schema, -Djava.awt.headless=true, -Djava.net.preferIPv4Stack=true, -Dpython.home=/usr/share/cmf/python, -XX:+UseConcMarkSweepGC, -XX:+UseParNewGC, -XX:+HeapDumpOnOutOfMemoryError, -Xmx2G, -XX:MaxPermSize=256m, -XX:+HeapDumpOnOutOfMemoryError, -XX:HeapDumpPath=/tmp, -XX:OnOutOfMemoryError=kill -9 %p], Args: [], Version: 5.8.3 (#8 built by jenkins on 20161019-1014 git: 518f0d6d44abc87bc392646e4369a20c8192b7cf)
[ec2-user@ip-172-31-15-71 ~]$ 

Line containing the phrase "Started Jetty Server"
[ec2-user@ip-172-31-15-71 ~]$ sudo cat /var/log/cloudera-scm-server/cloudera-scm-server.log | grep "Started Jetty server"
2017-07-06 11:35:30,627 INFO WebServerImpl:com.cloudera.server.cmf.WebServerImpl: Started Jetty server.
[ec2-user@ip-172-31-15-71 ~]$ 


Contents of db.properties file
[ec2-user@ip-172-31-15-71 ~]$ sudo cat /etc/cloudera-scm-server/db.properties
# Auto-generated by scm_prepare_database.sh on Do 6. Jul 11:32:32 EDT 2017
#
# For information describing how to configure the Cloudera Manager Server
# to connect to databases, see the "Cloudera Manager Installation Guide."
#
com.cloudera.cmf.db.type=mysql
com.cloudera.cmf.db.host=localhost
com.cloudera.cmf.db.name=oozie
com.cloudera.cmf.db.user=oozie
com.cloudera.cmf.db.password=oozie_password


```
