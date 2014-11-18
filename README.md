collectd-write-graphite
=======================

Basic collectd-based server monitoring. Sends stats to Graphite.

Collectd metrics:

* CPU used/free/idle/etc
* Free disk (via the .dockerinit filesystem)
* Load average
* Memory used/free/etc

Environment variables
---------------------

* `HOST_NAME`
  - Will be sent to Graphite
  - Required
* `GRAPHITE_HOST`
  - Graphite IP or hostname
  - Required
* `GRAPHITE_PORT`
  - Graphite port
  - Optional, defaults to 2003
* `INSTANCE_ID`
  - This is read from the AWS environment to give us a unique value for a cluster of servers
