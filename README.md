# mqtt-elasticSearch

This file stores data published on MQTT in elasticSearch

# Dependencie

Paho MQTT Python client library

`pip install paho-mqtt`

ElasticSearch client library

`pip install elasticsearch`

ElasticSearch must be running on the same server on port 9200

# Configuration :

Modify the header lines in the file to include the http or ip address and port of your mqtt server

```
mqttServer="localhost"
mqttPort="1883"
mqttLogin="mqtt"
mqttPassword="password"
```

Modify if required the topics (default $SYS topic)

```
#channelSubs="$SYS/#"
#channelSubs="temp_salon"
#use below as alternative to subscribe to all channels
channelSubs="#"
```

# use

Run as python mqtt-elasticSearch from terminal on the same machine where elasticSearch is running

`python3 /home/scripts/mqttToElasticSearch.py`
