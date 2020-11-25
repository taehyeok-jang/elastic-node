# elastic-node
A simple search engine for cities around the world.

Ref. 
https://www.digitalocean.com/community/tutorials/how-to-build-a-real-time-search-engine-with-node-vue-and-elasticsearch

## Prerequisites
- Docker 
- Node

## How to run
```
# initialize node 
npm init
npm install

# run es on docker
docker run -p 9200:9200 -p 9300:9300 -e "discovery.type=single-node" docker.elastic.co/elasticsearch/elasticsearch:7.8.1

# import cities.json into es 
node data.js
# run 
node index.js 
```
