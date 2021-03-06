# marathon

[![Join the chat at https://gitter.im/mesoscloud/marathon](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/mesoscloud/marathon?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Marathon

https://mesosphere.github.io/marathon/

## CentOS

[![](https://badge.imagelayers.io/mesoscloud/marathon:0.11.0-centos-7.svg)](https://imagelayers.io/?images=mesoscloud/marathon:0.11.0-centos-7)

e.g.

```
docker run -d \
-e MARATHON_HOSTNAME=ip.address \
-e MARATHON_HTTPS_ADDRESS=ip.address \
-e MARATHON_HTTP_ADDRESS=ip.address \
-e MARATHON_MASTER=zk://node-1:2181,node-2:2181,node-3:2181/mesos \
-e MARATHON_ZK=zk://node-1:2181,node-2:2181,node-3:2181/marathon \
--name marathon --net host --restart always mesoscloud/marathon:0.11.0-centos-7
```

Set environment variable `SECRET` to enable framework authentication.

## Ubuntu

[![](https://badge.imagelayers.io/mesoscloud/marathon:0.11.0-ubuntu-15.04.svg)](https://imagelayers.io/?images=mesoscloud/marathon:0.11.0-ubuntu-15.04)

e.g.

```
docker run -d \
-e MARATHON_HOSTNAME=ip.address \
-e MARATHON_HTTPS_ADDRESS=ip.address \
-e MARATHON_HTTP_ADDRESS=ip.address \
-e MARATHON_MASTER=zk://node-1:2181,node-2:2181,node-3:2181/mesos \
-e MARATHON_ZK=zk://node-1:2181,node-2:2181,node-3:2181/marathon \
--name marathon --net host --restart always mesoscloud/marathon:0.11.0-ubuntu-15.04
```

Set environment variable `SECRET` to enable framework authentication.
