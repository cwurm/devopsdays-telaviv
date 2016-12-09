# Using Elastic to monitor everything
DevOpsDays Tel Aviv

12 Dec 2016

### Download Metricbeat
Download from https://www.elastic.co/downloads/beats/metricbeat (7.2 MB)

### Edit `metricbeat.yml`
Edit these lines:
```
  hosts: ["localhost:9200"]
  
  [...]
  
  username: "elastic"
  password: "changeme"
```

Replace with the hostname, username and password of your Elasticsearch.

### Run Metricbeat
```
./metricbeat -e
```
