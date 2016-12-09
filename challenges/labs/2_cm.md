```
[root@sebcxinyi01 ~]# ls /etc/yum.repos.d
CentOS-Base.repo       CentOS-fasttrack.repo  CentOS-Vault.repo
CentOS-Debuginfo.repo  CentOS-Media.repo      mysql-community.repo
```

```
[root@sebcxinyi01 ~]# /usr/share/cmf/schema/scm_prepare_database.sh mysql -h 172.16.7.24 --scm-host sebcxinyi01 scm scm password
JAVA_HOME=/usr/lib/jvm/jre-openjdk
Verifying that we can write to /etc/cloudera-scm-server
Creating SCM configuration file in /etc/cloudera-scm-server
Executing:  /usr/lib/jvm/jre-openjdk/bin/java -cp /usr/share/java/mysql-connector-java.jar:/usr/share/java/oracle-connector-java.jar:/usr/share/cmf/schema/../lib/* com.cloudera.enterprise.dbutil.DbCommandExecutor /etc/cloudera-scm-server/db.properties com.cloudera.cmf.db.
log4j:ERROR Could not find value for key log4j.appender.A
log4j:ERROR Could not instantiate appender named "A".
[2016-12-08 20:25:31,673] INFO     0[main] - com.cloudera.enterprise.dbutil.DbCommandExecutor.testDbConnection(DbCommandExecutor.java) - Successfully connected to database.
All done, your SCM database is configured correctly!
```