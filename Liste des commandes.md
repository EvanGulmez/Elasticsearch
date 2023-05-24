Lundi - Jour 1 : Install Kibana with Docker

docker network create elastic
docker pull docker.elastic.co/elasticsearch/elasticsearch:8.7.1
docker run --name es-node01 --net elastic -p 9200:9200 -p 9300:9300 -t docker.elastic.co/elasticsearch/elasticsearch:8.7.1

ERROR: Elasticsearch exited unexpectedly

-> Solution :
docker run --name es-node01 --net elastic -p 9200:9200 -p 9300:9300 -e "discovery.type=single-node" -t docker.elastic.co/elasticsearch/elasticsearch:8.7.1

Sauvegarder les données telle que le password et le token pour se connecter a Kibana

Copier coller l'url générer en remplaçant "0.0.0.0" par "localhost"

Username : elastic et coller le mdp ainsi que le token pour se connecter  

