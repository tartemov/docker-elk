# elastic docker-compose

Run the latest version of the Elastic Products (Elasticsearch, Logstash, Kibana, APM) stack with Docker and Docker Compose.

Based on the official Docker images:

* [elasticsearch](https://github.com/elastic/elasticsearch-docker)
* [logstash](https://github.com/elastic/logstash-docker)
* [kibana](https://github.com/elastic/kibana-docker)
* [apm-server](https://github.com/elastic/apm-server)

# How to setup 

1. Clone this repository

2. Start the ELK stack using `docker-compose`:

```console
$ docker-compose up -d
```

Give Kibana a few seconds to initialize, then access the Kibana web UI by hitting [http://localhost:5601](http://localhost:5601) with a web browser.

By default, the stack exposes the following ports:
* 5000: Logstash TCP input.
* 9200: Elasticsearch HTTP
* 9300: Elasticsearch TCP transport
* 5601: Kibana
* 8200: APM-Server
