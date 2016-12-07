**version of the API**
```
[root@SEBCxinyi /]# curl -u cxinyi:cloudera 'http://52.163.49.151:7180/api/version'
v14
```

**CM version**
```
[root@SEBCxinyi /]# curl -u cxinyi:cloudera 'http://52.163.49.151:7180/api/v14/cm/version'
{
  "version" : "5.9.0",
  "buildUser" : "jenkins",
  "buildTimestamp" : "20161006-1801",
  "gitHash" : "898a5e032c080e18833dfc58180761f6ef2ea351",
  "snapshot" : false
}
```

**all CM users**
```
[root@SEBCxinyi /]# curl -u cxinyi:cloudera 'http://52.163.49.151:7180/api/v14/users'
{
  "items" : [ {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ]
  }, {
    "name" : "cxinyi",
    "roles" : [ "ROLE_ADMIN" ]
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ]
  } ]
}
```

**database server in use by CM**
```
[root@SEBCxinyi /]# curl -u cxinyi:cloudera 'http://52.163.49.151:7180/api/v14/cm/scmDbInfo'
{
  "scmDbType" : "MYSQL",
  "embeddedDbUsed" : false
}
```