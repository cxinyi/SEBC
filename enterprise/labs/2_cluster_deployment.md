```
[root@SEBCxinyi /]# curl -u cxinyi http://52.163.49.151:7180/api/v2/cm/deployment
Enter host password for user 'cxinyi':
{
  "timestamp" : "2016-12-07T06:23:50.151Z",
  "clusters" : [ {
    "name" : "cxinyi",
    "version" : "CDH5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "524288000"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "524288000"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "3995651276"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "672"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "SEBCxinyi"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "password"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-5c6ec80736fa76a29785074d0db640f4",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "0c520a8b-f627-4d0f-aeb7-0b4278982e44"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-5e35e46a6a975c2b9e4f4f2093b664cd",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "9f5279ee-8dbf-4248-9afd-3d1e6e704017"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-5f189312e342ded196249f04b2c51d21",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "75c6c955-bd11-4b59-b3bd-480faf024382"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-82893949480fea548a9ce88103f5f68d",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "810c5d39-fed2-47d3-8674-18a411f261e7"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-d8618a40fdfd9ebed88e36f3341a4cb0",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "c7caef2e-a7a3-4c02-a0f0-cf1bed3d912c"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-82893949480fea548a9ce88103f5f68d",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "810c5d39-fed2-47d3-8674-18a411f261e7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8codbfhznif7uwt09rk2yotzf"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-5c6ec80736fa76a29785074d0db640f4",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "0c520a8b-f627-4d0f-aeb7-0b4278982e44"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1hbjqt80d8dhlzf4d1ml7m1j2"
          } ]
        }
      } ],
      "displayName" : "Hive"
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "SERVER",
          "items" : [ {
            "name" : "zookeeper_server_java_heapsize",
            "value" : "524288000"
          } ]
        } ],
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-5c6ec80736fa76a29785074d0db640f4",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "0c520a8b-f627-4d0f-aeb7-0b4278982e44"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "781gc2p2h8gaymlsqyssp1q3s"
          }, {
            "name" : "serverId",
            "value" : "3"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-82893949480fea548a9ce88103f5f68d",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "810c5d39-fed2-47d3-8674-18a411f261e7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6e7k7cioeqw5ryi5eomqtp0kx"
          }, {
            "name" : "serverId",
            "value" : "2"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-d8618a40fdfd9ebed88e36f3341a4cb0",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "c7caef2e-a7a3-4c02-a0f0-cf1bed3d912c"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "35nhk3rxm7mjkmkovgdc6aoc6"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        }
      } ],
      "displayName" : "ZooKeeper"
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "database_host",
          "value" : "SEBCxinyi"
        }, {
          "name" : "database_password",
          "value" : "password"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-NAMENODE-82893949480fea548a9ce88103f5f68d"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-5e35e46a6a975c2b9e4f4f2093b664cd",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "9f5279ee-8dbf-4248-9afd-3d1e6e704017"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8dl89h1mmpab4jzb6vyxy94q4"
          }, {
            "name" : "secret_key",
            "value" : "cYzqo0SYVV4FyuKf4nAf2k22DA0Uct"
          } ]
        }
      } ],
      "displayName" : "Hue"
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "OOZIE_SERVER",
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "SEBCxinyi"
          }, {
            "name" : "oozie_database_password",
            "value" : "password"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
          }, {
            "name" : "oozie_java_heapsize",
            "value" : "524288000"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-82893949480fea548a9ce88103f5f68d",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "810c5d39-fed2-47d3-8674-18a411f261e7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "akg6sh4y2tplb5sazgvfros0p"
          } ]
        }
      } ],
      "displayName" : "Oozie"
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "8"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "2"
          } ]
        }, {
          "roleType" : "JOBHISTORY",
          "items" : [ {
            "name" : "mr2_jobhistory_java_heapsize",
            "value" : "524288000"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "rm_cpu_shares",
            "value" : "1800"
          }, {
            "name" : "rm_io_weight",
            "value" : "900"
          }, {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/mnt/resource/yarn/nm,/var/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/mnt/resource/yarn/container-logs,/var/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "3"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "1024"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "resource_manager_java_heapsize",
            "value" : "524288000"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "4483"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "3"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "90"
        }, {
          "name" : "yarn_service_cgroups",
          "value" : "false"
        }, {
          "name" : "yarn_service_lce_always",
          "value" : "false"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "kOEpSjhRyLIMIq1h848Znh5Cm23x0f"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-82893949480fea548a9ce88103f5f68d",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "810c5d39-fed2-47d3-8674-18a411f261e7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3zjti7m6dqlbsqg98nam2zir6"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-5c6ec80736fa76a29785074d0db640f4",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "0c520a8b-f627-4d0f-aeb7-0b4278982e44"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "c8uarmzye7bhhj38uxa5s9efg"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-5f189312e342ded196249f04b2c51d21",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "75c6c955-bd11-4b59-b3bd-480faf024382"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4i464uibkcdxjpbbmvwlnv4fb"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-82893949480fea548a9ce88103f5f68d",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "810c5d39-fed2-47d3-8674-18a411f261e7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "507r3zgr093nvddj0lg27gy8w"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-d8618a40fdfd9ebed88e36f3341a4cb0",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "c7caef2e-a7a3-4c02-a0f0-cf1bed3d912c"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5b62ouqpclwf861hzfdxhkq3r"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-82893949480fea548a9ce88103f5f68d",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "810c5d39-fed2-47d3-8674-18a411f261e7"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "149"
          }, {
            "name" : "role_jceks_password",
            "value" : "bldpi9gsue8217qkuot236jdx"
          } ]
        }
      } ],
      "displayName" : "YARN (MR2 Included)"
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "BALANCER",
          "items" : [ {
            "name" : "balancer_java_heapsize",
            "value" : "524288000"
          } ]
        }, {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "datanode_java_heapsize",
            "value" : "1073741824"
          }, {
            "name" : "dfs_data_dir_list",
            "value" : "/mnt/resource/dfs/dn,/var/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "3104312115"
          }, {
            "name" : "dfs_datanode_failed_volumes_tolerated",
            "value" : "1"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4294967296"
          }, {
            "name" : "rm_cpu_shares",
            "value" : "200"
          }, {
            "name" : "rm_io_weight",
            "value" : "100"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "JOURNALNODE",
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/var/jn"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/mnt/resource/dfs/nn,/var/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          }, {
            "name" : "namenode_java_heapsize",
            "value" : "524288000"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/mnt/resource/dfs/snn"
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "524288000"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "8xKvt0Ngm9wHyur7bVgpoS3VlIJEOy"
        }, {
          "name" : "dfs_ha_fencing_methods",
          "value" : "shell(true)"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "sQOOpcy5pJFlF1eoTlJ6CAYHVhuaY4"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "VCvM7NdXz0krjAYBlBOjVJmCzW6ONw"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "10"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-5e35e46a6a975c2b9e4f4f2093b664cd",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "9f5279ee-8dbf-4248-9afd-3d1e6e704017"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-5c6ec80736fa76a29785074d0db640f4",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "0c520a8b-f627-4d0f-aeb7-0b4278982e44"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2w36pn5z1gxgnh18ax76pmue2"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-5f189312e342ded196249f04b2c51d21",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "75c6c955-bd11-4b59-b3bd-480faf024382"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2r8jsdrtyix0oyjbcg5pvmj8y"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-82893949480fea548a9ce88103f5f68d",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "810c5d39-fed2-47d3-8674-18a411f261e7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5tbmuzjr14nliim8241hw5xnr"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-d8618a40fdfd9ebed88e36f3341a4cb0",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "c7caef2e-a7a3-4c02-a0f0-cf1bed3d912c"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "aiunlfv5evsegvb1hujohpdai"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-5c6ec80736fa76a29785074d0db640f4",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "0c520a8b-f627-4d0f-aeb7-0b4278982e44"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2w502y4omthjgyk3reqfxcohl"
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-82893949480fea548a9ce88103f5f68d",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "810c5d39-fed2-47d3-8674-18a411f261e7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "34b099dzcg683a9xk7k75gkuv"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-5c6ec80736fa76a29785074d0db640f4",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "0c520a8b-f627-4d0f-aeb7-0b4278982e44"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ctgp2z6j4olpf8z1ygsvbfajb"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-82893949480fea548a9ce88103f5f68d",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "810c5d39-fed2-47d3-8674-18a411f261e7"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4bi359u8yke1k9k8hantg4isa"
          } ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-d8618a40fdfd9ebed88e36f3341a4cb0",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "c7caef2e-a7a3-4c02-a0f0-cf1bed3d912c"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7s7u0akcjgzlcaepngph2z587"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-5c6ec80736fa76a29785074d0db640f4",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "0c520a8b-f627-4d0f-aeb7-0b4278982e44"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "165"
          }, {
            "name" : "role_jceks_password",
            "value" : "4b32glr7a7mpuducuafohmtqe"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-82893949480fea548a9ce88103f5f68d",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "810c5d39-fed2-47d3-8674-18a411f261e7"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true"
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1"
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1"
          }, {
            "name" : "namenode_id",
            "value" : "157"
          }, {
            "name" : "nameservice_mountpoints",
            "value" : "/"
          }, {
            "name" : "role_jceks_password",
            "value" : "2d3nlf179o7uv5l77ptfmkib8"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "9f5279ee-8dbf-4248-9afd-3d1e6e704017",
    "ipAddress" : "172.16.7.7",
    "hostname" : "SEBCxinyi",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "810c5d39-fed2-47d3-8674-18a411f261e7",
    "ipAddress" : "172.16.7.10",
    "hostname" : "SEBCxinyi-01",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "0c520a8b-f627-4d0f-aeb7-0b4278982e44",
    "ipAddress" : "172.16.7.11",
    "hostname" : "SEBCxinyi-02",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "c7caef2e-a7a3-4c02-a0f0-cf1bed3d912c",
    "ipAddress" : "172.16.7.12",
    "hostname" : "SEBCxinyi-03",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "75c6c955-bd11-4b59-b3bd-480faf024382",
    "ipAddress" : "172.16.7.13",
    "hostname" : "SEBCxinyi-04",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-ACTIVITYMONITOR-5e35e46a6a975c2b9e4f4f2093b664cd",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "2bccb5c22154abc133364227dfdd9a9cff49a04e490ca30da203396e2be0340e",
    "pwSalt" : -6110439684505101348,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-5e35e46a6a975c2b9e4f4f2093b664cd",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "7695fbe5612969d1ed2c5b34174d4bb0358b2bece27b223131250d4e418a5ee5",
    "pwSalt" : -1338415794508202651,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-5e35e46a6a975c2b9e4f4f2093b664cd",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "f0a822bc38b51df6498a0fdf5615ef9b9188e4b157711fd02a8f365564c15e89",
    "pwSalt" : -6068812985558371488,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-5e35e46a6a975c2b9e4f4f2093b664cd",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "b0854fdb50476172e1e1dec0815a5d2e19f12ad9b989ea3462519db9603322d0",
    "pwSalt" : -5088181089670733446,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-5e35e46a6a975c2b9e4f4f2093b664cd",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "fb3d64bd14bc3c026028a8c2330521fa41bb734f60b4c22ac90ad1652dde60bb",
    "pwSalt" : 1277393868481638976,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_LIMITED" ],
    "pwHash" : "4a50ed335d2b5b3bc8223b57d4807ded3e4ca0584be8e10cb2688b36bbeb8dd6",
    "pwSalt" : -5246071989141541408,
    "pwLogin" : true
  }, {
    "name" : "cxinyi",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "09cdf03f496b39bc8ee5e83b7d3be56b191a413f132637002f749a47697449d2",
    "pwSalt" : 4829791594820678543,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "54aebd5221a2249bedfaaab65aa00e0b9f6a2cc4bee7e935f84add83dac4705b",
    "pwSalt" : 344322282626015184,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.8.2",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20160916-1426",
    "gitHash" : "d23c620f3a3bbd85d8511d6ebba49beaaab14b75",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "ACTIVITYMONITOR",
        "items" : [ {
          "name" : "firehose_database_host",
          "value" : "SEBCxinyi"
        }, {
          "name" : "firehose_database_name",
          "value" : "amon"
        }, {
          "name" : "firehose_database_password",
          "value" : "amon"
        }, {
          "name" : "firehose_database_user",
          "value" : "amon"
        }, {
          "name" : "firehose_heapsize",
          "value" : "524288000"
        } ]
      }, {
        "roleType" : "EVENTSERVER",
        "items" : [ {
          "name" : "event_server_heapsize",
          "value" : "524288000"
        } ]
      }, {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "524288000"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "SEBCxinyi"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "password"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        }, {
          "name" : "headlamp_heapsize",
          "value" : "524288000"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "524288000"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ACTIVITYMONITOR-5e35e46a6a975c2b9e4f4f2093b664cd",
      "type" : "ACTIVITYMONITOR",
      "hostRef" : {
        "hostId" : "9f5279ee-8dbf-4248-9afd-3d1e6e704017"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "d74ie5tba1jjowphho8iapcjl"
        } ]
      }
    }, {
      "name" : "mgmt-ALERTPUBLISHER-5e35e46a6a975c2b9e4f4f2093b664cd",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "9f5279ee-8dbf-4248-9afd-3d1e6e704017"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "ddcl8cbgjofu4q2w5ysjqu2fn"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-5e35e46a6a975c2b9e4f4f2093b664cd",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "9f5279ee-8dbf-4248-9afd-3d1e6e704017"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "f0bpq1hr2z9az70kmkl8qqgj2"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-5e35e46a6a975c2b9e4f4f2093b664cd",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "9f5279ee-8dbf-4248-9afd-3d1e6e704017"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "9izva453b4a5xex0jargndcvx"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-5e35e46a6a975c2b9e4f4f2093b664cd",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "9f5279ee-8dbf-4248-9afd-3d1e6e704017"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "dk1d6ooekisqn81z5cqlqzc82"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-5e35e46a6a975c2b9e4f4f2093b664cd",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "9f5279ee-8dbf-4248-9afd-3d1e6e704017"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "5oufr9tqxk63a2ajuts0elbgs"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/25/2012 20:40"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "NOT_ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "http://archive.cloudera.com/cdh5/parcels/5.8.2/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
    } ]
  }
```