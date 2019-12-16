2019-11-29T09:08:10Z E! [outputs.influxdb] when writing to [http://localhost:8086]: 500 Internal Server Error: [shard 31] open /var/lib/influxdb/wal/sensors/autogen/31/_00006.wal: permission denied
2019-11-29T09:08:10Z E! [agent] Error writing to output [influxdb]: could not write any address

解决办法:
chown -R influxdb:influxdb /var/lib/influxdb/

