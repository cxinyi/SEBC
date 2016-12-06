```
**Delete the directory**
[hdfs@SEBCxinyi ~]$ hdfs dfs -rm -r /precious
rm: Failed to move to trash: hdfs://SEBCxinyi:8020/precious: The directory /precious cannot be deleted since /precious is snapshottable and already has snapshots


**Delete the text file**
[hdfs@SEBCxinyi ~]$ hdfs dfs -rm -r /precious/hello.txt
16/12/06 02:33:15 INFO fs.TrashPolicyDefault: Moved: 'hdfs://SEBCxinyi:8020/precious/hello.txt' to trash at: hdfs://SEBCxinyi:8020/user/hdfs/.Trash/Current/precious/hello.txt


**Restore the deleted file**
hdfs dfs -cp precious/.snapshot/sebc-hdfs-test/hello.txt precious
```