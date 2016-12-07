**Stop**
```
[root@SEBCxinyi /]# curl -u cxinyi:cloudera -X POST 'http://52.163.49.151:7180/api/v12/clusters/cxinyi/services/hive/commands/stop'
{
  "id" : 1248,
  "name" : "Stop",
  "startTime" : "2016-12-07T06:46:45.538Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}
```

**Start**
```
[root@SEBCxinyi /]# curl -u cxinyi:cloudera -X POST 'http://52.163.49.151:7180/api/v12/clusters/cxinyi/services/hive/commands/start'
{
  "id" : 1252,
  "name" : "Start",
  "startTime" : "2016-12-07T06:47:50.741Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }
}
```

**Check**
```
[root@SEBCxinyi /]# curl -u cxinyi:cloudera -X GET 'http://52.163.49.151:7180/api/v12/clusters/cxinyi/services/hive'
{
  "name" : "hive",
  "type" : "HIVE",
  "clusterRef" : {
    "clusterName" : "cluster"
  },
  "serviceUrl" : "http://SEBCxinyi:7180/cmf/serviceRedirect/hive",
  "roleInstancesUrl" : "http://SEBCxinyi:7180/cmf/serviceRedirect/hive/instances",
  "serviceState" : "STARTED",
  "healthSummary" : "GOOD",
  "healthChecks" : [ {
    "name" : "HIVE_HIVEMETASTORES_HEALTHY",
    "summary" : "GOOD",
    "suppressed" : false
  }, {
    "name" : "HIVE_HIVESERVER2S_HEALTHY",
    "summary" : "GOOD",
    "suppressed" : false
  } ],
  "configStalenessStatus" : "FRESH",
  "clientConfigStalenessStatus" : "FRESH",
  "maintenanceMode" : false,
  "maintenanceOwners" : [ ],
  "displayName" : "Hive",
  "entityStatus" : "GOOD_HEALTH"
}
```