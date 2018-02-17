# logspout to elasticsearch and kibana for sample docker compose

## Using service list

* logspout: [https://github.com/gliderlabs/logspout](https://github.com/gliderlabs/logspout)
* logstash: [https://www.elastic.co/en/products/logstash](https://www.elastic.co/en/products/logstash)
* elasticsearch: [https://www.elastic.co/products/elasticsearch](https://www.elastic.co/products/elasticsearch)
* kibana: [https://www.elastic.co/products/kibana](https://www.elastic.co/products/kibana)


## Usage

```
$ docker-compose up -d

# Check kibana started.
$ docker-compose logs kibana
```

Access to http://localhost:5601.

### Note

* For Docker for Windows or Mac, set dedicated memory size > 4GB

