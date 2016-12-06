**Source Directory**
```
[hduser@SEBCxinyi ~]$ hdfs fsck /testSource -files -blocks
Connecting to namenode via http://SEBCxinyi:50070
FSCK started by hduser (auth:SIMPLE) from /172.16.7.7 for path /testSource at Mon Dec 05 23:14:31 CST 2016
/testSource <dir>
/testSource/terasort-inputrob <dir>
/testSource/terasort-inputrob/_SUCCESS 0 bytes, 0 block(s):  OK

/testSource/terasort-inputrob/part-m-00000 524288000 bytes, 4 block(s):  OK
0. BP-384511601-172.16.7.7-1480995778346:blk_1073742564_1740 len=134217728 Live_repl=3
1. BP-384511601-172.16.7.7-1480995778346:blk_1073742565_1741 len=134217728 Live_repl=3
2. BP-384511601-172.16.7.7-1480995778346:blk_1073742567_1743 len=134217728 Live_repl=3
3. BP-384511601-172.16.7.7-1480995778346:blk_1073742568_1744 len=121634816 Live_repl=3

Status: HEALTHY
 Total size:    524288000 B
 Total dirs:    2
 Total files:   2
 Total symlinks:                0
 Total blocks (validated):      4 (avg. block size 131072000 B)
 Minimally replicated blocks:   4 (100.0 %)
 Over-replicated blocks:        0 (0.0 %)
 Under-replicated blocks:       0 (0.0 %)
 Mis-replicated blocks:         0 (0.0 %)
 Default replication factor:    3
 Average block replication:     3.0
 Corrupt blocks:                0
 Missing replicas:              0 (0.0 %)
 Number of data-nodes:          4
 Number of racks:               1
FSCK ended at Mon Dec 05 23:14:31 CST 2016 in 1 milliseconds


The filesystem under path '/testSource' is HEALTHY
```

**Target Directory**
```
[hduser@SEBCxinyi ~]$ hdfs fsck /test -files -blocks
Connecting to namenode via http://SEBCxinyi:50070
FSCK started by hduser (auth:SIMPLE) from /172.16.7.7 for path /test at Mon Dec 05 23:13:59 CST 2016
/test <dir>
/test/terasort-input <dir>
/test/terasort-input/_SUCCESS 0 bytes, 0 block(s):  OK

/test/terasort-input/part-m-00000 262144000 bytes, 2 block(s):  OK
0. BP-384511601-172.16.7.7-1480995778346:blk_1073742558_1734 len=134217728 Live_repl=3
1. BP-384511601-172.16.7.7-1480995778346:blk_1073742561_1737 len=127926272 Live_repl=3

/test/terasort-input/part-m-00001 262144000 bytes, 2 block(s):  OK
0. BP-384511601-172.16.7.7-1480995778346:blk_1073742560_1736 len=134217728 Live_repl=3
1. BP-384511601-172.16.7.7-1480995778346:blk_1073742562_1738 len=127926272 Live_repl=3

Status: HEALTHY
 Total size:    524288000 B
 Total dirs:    2
 Total files:   3
 Total symlinks:                0
 Total blocks (validated):      4 (avg. block size 131072000 B)
 Minimally replicated blocks:   4 (100.0 %)
 Over-replicated blocks:        0 (0.0 %)
 Under-replicated blocks:       0 (0.0 %)
 Mis-replicated blocks:         0 (0.0 %)
 Default replication factor:    3
 Average block replication:     3.0
 Corrupt blocks:                0
 Missing replicas:              0 (0.0 %)
 Number of data-nodes:          4
 Number of racks:               1
FSCK ended at Mon Dec 05 23:13:59 CST 2016 in 3 milliseconds


The filesystem under path '/test' is HEALTHY
```