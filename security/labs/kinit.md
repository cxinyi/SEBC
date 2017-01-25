```
[root@SEBCxinyi ~]# kinit cxinyi
Password for cxinyi@SEBCxinyi:
[root@SEBCxinyi ~]# klist
Ticket cache: FILE:/tmp/krb5cc_0
Default principal: cxinyi@SEBCxinyi

Valid starting     Expires            Service principal
12/07/16 21:27:15  12/08/16 21:27:15  krbtgt/SEBCxinyi@SEBCxinyi
        renew until 12/07/16 21:27:15
```

Notice you have a non-renewable ticket here: the `Valid Starting` and `renew until` fields have the same value.
