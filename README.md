# monitoring dashboards
backup of grafana dashboards


### setup
The nodejs package "wizzy" uses the grafana api to extract the dashboards and other data.

```
npm install -g wizzy
# create conf/wizzy.conf with auth:
wizzy set grafana url https://grafana.fqdn
wizzy set grafana username GRAFANA_USERNAME
wizzy set grafana password GRAFANA_PASSWORD
```


### backup process

```
wizzy import dashboards
git add dashboards
git commit
```


### alternatives
* https://github.com/ysde/grafana-backup-tool
* Manually export and commit the json for dashboards
