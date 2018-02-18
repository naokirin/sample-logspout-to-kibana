# logspout to elasticsearch and kibana for sample docker compose

## Using service list

* Logspout: [https://github.com/gliderlabs/logspout](https://github.com/gliderlabs/logspout)
* Logstash: [https://www.elastic.co/en/products/logstash](https://www.elastic.co/en/products/logstash)
* Elasticsearch: [https://www.elastic.co/products/elasticsearch](https://www.elastic.co/products/elasticsearch)
* Kibana: [https://www.elastic.co/products/kibana](https://www.elastic.co/products/kibana)
* Curator: [https://www.elastic.co/guide/en/elasticsearch/client/curator/current/index.html](https://www.elastic.co/guide/en/elasticsearch/client/curator/current/index.html)

## Usage

### Old indeces deletion setting

* edit cron duration and filters in `elasticsearch\_old\_index\_deletion/Dockerfile`
  - https://github.com/naokirin/sample-logspout-to-kibana/blob/master/elasticsearch_old_index_deletion/Dockerfile#L15

### Start containers

```
$ docker-compose build
$ docker-compose up -d

# Check kibana started.
$ docker-compose logs kibana
```

Access to http://localhost:5601.

### Note

* For Docker for Windows or Mac, set dedicated memory size > 4GB

