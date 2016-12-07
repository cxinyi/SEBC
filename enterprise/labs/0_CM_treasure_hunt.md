**What is ubertask optimization?**
```
Enable MapReduce to runs "sufficiently small" jobs sequentially within a single JVM.
```

**Where in CM is the Kerberos Security Realm value displayed?**
```
Under Administration->Settings, Category->Kerberos
```

**Which CDH service(s) host a property for enabling Kerberos authentication?**
```
Cloudera Manager
```

**How do you upgrade the CM agents?**
```
1. Stop CM Services
2. Stop cluster
3. Stop CM Server and Agent.
4. Edit the cloudera manager repo file
5. Type "sudo yum clean all"
6. Type "sudo yum upgrade cloudera-scm-agent"
7. Start CM Server.
8. Using the upgrade wizard, upgrade the Cloudera Manager Agent.
```

**Give the tsquery statement used to chart Hue's CPU utilization?**
```
select cpu_percent_across_hosts where roleType=HUE_SERVER
```

**Name all the roles that make up the Hive service**
```
Hive Metastore Server
HiveServer2
```

**What steps must be completed before integrating Cloudera Manager with Kerberos?**
```
Set up a working KDC.

The KDC should be configured to have non-zero ticket lifetime and renewal lifetime.

OpenLdap client libraries should be installed on the Cloudera Manager Server host if you want to use Active Directory. 
Also, Kerberos client libraries should be installed on ALL hosts.

Cloudera Manager needs an account that has permissions to create other accounts in the KDC.
```
