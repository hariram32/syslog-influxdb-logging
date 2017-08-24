# syslog-influxdb-logging
sample config files to use sysylog to export data to influxdb
syslog-ng.conf-influx-server influxdb server running syslog
syslog-ng.conf-central-syslog on central syslog server
haproxy.cfg ha proxy config server (adapt to paticular front ends & backends)
syslog-ng.conf syslog running on ha proxies
in this example an HA Proxy uses syslog to log data to two central syslog servers. Data is filtered to 2 influxdb servers. It is then possible to use Grafana to monitor performance & metrics on a dashboard. See https://github.com/mbadley/grafana-telegraf-influxdb for sample dashboards.
