# ansible-roles

example

```
- hosts: zookeeper
  vars:
    zookeeperZooCfg:
      dataDir: "/var/lib/zookeeper"
      servers:
        - {host: "10.46.70.134", ports: "2888:3888" }
        - {host: "10.46.71.180", ports: "2888:3888" }
        - {host: "10.46.68.164", ports: "2888:3888" }

  roles:
    - java
    - zookeeper
```