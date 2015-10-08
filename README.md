# ansible-roles

example

```
- hosts: zookeeper
  vars:
    zookeeperZooCfg:
      dataDir: "/var/lib/zookeeper"
      servers:
        - {host: "ip1", ports: "2888:3888" }
        - {host: "ip2", ports: "2888:3888" }
        - {host: "ip3", ports: "2888:3888" }

  roles:
    - java
    - zookeeper
```