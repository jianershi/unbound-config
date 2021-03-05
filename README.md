# Unbound Config

unbound panel: https://grafana.com/grafana/dashboards/11705

## Steps

1. install and config unbound, including setup new control certificate for the server (needed when exporting the stats with unbound_exporter)
2. install Grafana
3. install PROMETHEUS
4. compile unbound_exporter and install the executable to /usr/bin /usr/sbin, which export command line unbound_control stats to web api
5. install the unbound_exporter as a systemd service
6. config PROMETHEUS file to use unbound_exporter as a source
7. add data source -> prometheus in grafana web panel
8. install unbound panel
