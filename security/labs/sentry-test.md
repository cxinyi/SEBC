**no authorizations**
```
beeline> !connect jdbc:hive2://172.16.7.11:10000/default;principal=hive/sebcxinyi-02@SEBCxinyi
scan complete in 2ms
Connecting to jdbc:hive2://172.16.7.11:10000/default;principal=hive/sebcxinyi-02@SEBCxinyi
Enter username for jdbc:hive2://172.16.7.11:10000/default;principal=hive/sebcxinyi-02@SEBCxinyi: cxinyi
Enter password for jdbc:hive2://172.16.7.11:10000/default;principal=hive/sebcxinyi-02@SEBCxinyi: ********
Connected to: Apache Hive (version 1.1.0-cdh5.8.2)
Driver: Hive JDBC (version 1.1.0-cdh5.8.2)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://172.16.7.11:10000/default> show tables;
INFO  : Compiling command(queryId=hive_20161208022828_5651e01f-455e-4b81-b5a1-a5dd9b68b9c5): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20161208022828_5651e01f-455e-4b81-b5a1-a5dd9b68b9c5); Time taken: 0.053 seconds
INFO  : Executing command(queryId=hive_20161208022828_5651e01f-455e-4b81-b5a1-a5dd9b68b9c5): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20161208022828_5651e01f-455e-4b81-b5a1-a5dd9b68b9c5); Time taken: 0.12 seconds
INFO  : OK
+-----------+--+
| tab_name  |
+-----------+--+
+-----------+--+
No rows selected (0.285 seconds)
```

**with authorizations**
```
0: jdbc:hive2://172.16.7.11:10000/default> show tables;
INFO  : Compiling command(queryId=hive_20161208024747_503bad00-f6f8-493d-951d-ae39090b4b2e): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20161208024747_503bad00-f6f8-493d-951d-ae39090b4b2e); Time taken: 0.068 seconds
INFO  : Executing command(queryId=hive_20161208024747_503bad00-f6f8-493d-951d-ae39090b4b2e): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20161208024747_503bad00-f6f8-493d-951d-ae39090b4b2e); Time taken: 0.121 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| persons    |
| sample_07  |
+------------+--+
2 rows selected (0.301 seconds)
```

**kinit as george**
```
0: jdbc:hive2://172.16.7.11:10000/default> SHOW TABLES;
INFO  : Compiling command(queryId=hive_20161208023939_32764356-d2b6-4d0c-86f8-36fb505d4a4b): SHOW TABLES
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20161208023939_32764356-d2b6-4d0c-86f8-36fb505d4a4b); Time taken: 0.056 seconds
INFO  : Executing command(queryId=hive_20161208023939_32764356-d2b6-4d0c-86f8-36fb505d4a4b): SHOW TABLES
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20161208023939_32764356-d2b6-4d0c-86f8-36fb505d4a4b); Time taken: 0.119 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| persons    |
| sample_07  |
+------------+--+
2 rows selected (0.285 seconds)
0: jdbc:hive2://172.16.7.11:10000/default>
```

**kinit as ferdinand**
```
[root@sebcxinyi ~]# kinit ferdinand
Password for ferdinand@SEBCxinyi:
[root@sebcxinyi ~]# beeline
Beeline version 1.1.0-cdh5.8.2 by Apache Hive
beeline> !connect jdbc:hive2://172.16.7.11:10000/default;principal=hive/sebcxinyi-02@SEBCxinyi
scan complete in 3ms
Connecting to jdbc:hive2://172.16.7.11:10000/default;principal=hive/sebcxinyi-02@SEBCxinyi
Enter username for jdbc:hive2://172.16.7.11:10000/default;principal=hive/sebcxinyi-02@SEBCxinyi: ferdinand
Enter password for jdbc:hive2://172.16.7.11:10000/default;principal=hive/sebcxinyi-02@SEBCxinyi: ********
Connected to: Apache Hive (version 1.1.0-cdh5.8.2)
Driver: Hive JDBC (version 1.1.0-cdh5.8.2)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://172.16.7.11:10000/default> show tables;
INFO  : Compiling command(queryId=hive_20161208024242_7771c0f2-529e-4c82-8496-4db1ef342c43): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20161208024242_7771c0f2-529e-4c82-8496-4db1ef342c43); Time taken: 0.054 seconds
INFO  : Executing command(queryId=hive_20161208024242_7771c0f2-529e-4c82-8496-4db1ef342c43): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20161208024242_7771c0f2-529e-4c82-8496-4db1ef342c43); Time taken: 0.123 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| sample_07  |
+------------+--+
1 row selected (0.288 seconds)
```
