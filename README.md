# Synology_dashboard_grafana
A grafana dashboard for monitoring Synology NAS

Dependencies
InfluxDB as the time-series database
Telegraf as the collector

Quick Start
- Enable SNMP on your Synology NAS
- Merge input_syno_telegraf.conf with your local Telegraf instance configuration (or create a new instance)
- Edit the SNMP 'public' string as appropriate
- Edit the 'agents' list to include all of your monitored NAS
- If you do not already have an InfluxDB output configured in your Telegraf instance:
- Merge the included output_influxdb_telegraf.conf  with your local Telegraf instance configuration:
- Edit the URL to your new InfluxDB instance
- Edit the username and password for this InfluxDB instance as appropriate
- Restart Telegraf

