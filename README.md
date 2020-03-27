# ELK Docker-compose repo

I create this repository because I use this as part of my home infrastructure. 

## Installation

Pull images:  
```
$ docker-compose pull  
```

Run containers in background:  
Linux:  
```
$ URL="localhost" docker-compose up -d  
```
Windows:  
```
$ $env:URL="localhost"; docker-compose up -d  
```

Metricbeats:  
```
https://www.elastic.co/guide/en/beats/metricbeat/current/metricbeat-installation.html
```
Change output.elasticsearch.hosts to elasticsearch url at ```metricbeat.yml``` file.  
Copy ```metricbeat.yml``` to ``` /etc/metricbeat/```.


## Access
Kibana is available on http://localhost/  
Elasticsearch is available on http://localhost:9200/