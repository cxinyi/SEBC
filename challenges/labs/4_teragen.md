**/user**
```
[hdfs@sebcxinyi00 ~]$ hdfs dfs -ls /user
Found 6 items
drwxrwxrwx   - mapred  hadoop           0 2016-12-08 20:51 /user/history
drwxrwxr-t   - hive    hive             0 2016-12-08 20:52 /user/hive
drwxrwxr-x   - hue     hue              0 2016-12-08 20:53 /user/hue
drwxrwxr-x   - oozie   oozie            0 2016-12-08 20:53 /user/oozie
drwxr-xr-x   - orchard orchard          0 2016-12-08 20:56 /user/orchard
drwxr-xr-x   - raffles raffles          0 2016-12-08 20:56 /user/raffles
```


**API**
```
[hdfs@sebcxinyi00 ~]$ curl -u 'admin:admin' http://172.16.7.20:7180/api/v12/host                                                                                        s
{
  "items" : [ {
    "hostId" : "a881aae8-7da6-4e1a-af43-0b62e6f6925f",
    "ipAddress" : "172.16.7.24",
    "hostname" : "sebcxinyi00",
    "rackId" : "/default",
    "hostUrl" : "http://sebcxinyi01:7180/cmf/hostRedirect/a881aae8-7da6-4e1a-af4                                                                                        3-0b62e6f6925f",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 4,
    "totalPhysMemBytes" : 14734823424
  }, {
    "hostId" : "343784de-5535-4c64-acb9-d85bc2bf86a4",
    "ipAddress" : "172.16.7.20",
    "hostname" : "sebcxinyi01",
    "rackId" : "/default",
    "hostUrl" : "http://sebcxinyi01:7180/cmf/hostRedirect/343784de-5535-4c64-acb                                                                                        9-d85bc2bf86a4",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 4,
    "totalPhysMemBytes" : 14734823424
  }, {
    "hostId" : "2a2a0563-0e98-4efb-b8e0-394c1dbfb4c4",
    "ipAddress" : "172.16.7.21",
    "hostname" : "sebcxinyi02",
    "rackId" : "/default",
    "hostUrl" : "http://sebcxinyi01:7180/cmf/hostRedirect/2a2a0563-0e98-4efb-b8e                                                                                        0-394c1dbfb4c4",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 4,
    "totalPhysMemBytes" : 14734823424
  }, {
    "hostId" : "b241f50a-6d16-4cc7-bed7-f68a3e0baca9",
    "ipAddress" : "172.16.7.22",
    "hostname" : "sebcxinyi03",
    "rackId" : "/default",
    "hostUrl" : "http://sebcxinyi01:7180/cmf/hostRedirect/b241f50a-6d16-4cc7-bed                                                                                        7-f68a3e0baca9",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 4,
    "totalPhysMemBytes" : 14734823424
  }, {
    "hostId" : "aa553abd-10f5-4972-81e2-3f0859613e58",
    "ipAddress" : "172.16.7.23",
    "hostname" : "sebcxinyi04",
    "rackId" : "/default",
    "hostUrl" : "http://sebcxinyi01:7180/cmf/hostRedirect/aa553abd-10f5-4972-81e                                                                                        2-3f0859613e58",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 4,
    "totalPhysMemBytes" : 14734823424
  } ]
```