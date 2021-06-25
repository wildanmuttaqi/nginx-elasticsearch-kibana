# Nginx ElasticSearch and Kibana with Docker

<img src="https://miro.medium.com/max/700/1*ZsZbAu4CawTm44lv4tycXA.png" height="200" />

# Setup
Set `vm.max_map_count` to at least 262144 :
```
grep vm.max_map_count /etc/sysctl.conf
vm.max_map_count=262144
```
to apply :
```
sysctl -w vm.max_map_count=262144
```

# Run 
Running `docker-compose.yml` :
```
docker-compose up -d
```

# Overview
![image](https://user-images.githubusercontent.com/73166558/123391140-e90aba00-d5c5-11eb-811c-f6025f49c284.png)
![image](https://user-images.githubusercontent.com/73166558/123391517-50286e80-d5c6-11eb-924e-a388dc382f62.png)

Reference :

- https://edward-cernera.medium.com/deploy-a-multi-node-elasticsearch-instance-with-docker-compose-ef63625f246e
- https://www.elastic.co/guide/en/elastic-stack-get-started/current/get-started-docker.html
