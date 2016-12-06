**teragen**
```

time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen -Dmapred.map.tasks=4 -D dfs.blocksize=32m 100000000 /user/cxinyi/terasort-input

real    2m6.620s
user    1m48.681s
sys     0m6.485s
```

**teragen**
```
time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort -Dmapred.map.tasks.speculative.execution=false terasort terasort_out 

real    5m23.311s
user    4m27.858s
sys     0m14.645s

```