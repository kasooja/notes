#[Basic Concepts | Elasticsearch Reference [5.0] | Elastic](https://www.elastic.co/guide/en/elasticsearch/reference/5.0/_basic_concepts.html#_cluster)

## Red
* replica

* near real time

* node

* cluster

* index

* type

* document

* shards

## Yellow
* replica shard is never allocated on the same node as the original/primary shard

* The number of shards and replicas can be defined per index at the time the index is created.

* After the index is created, you may change the number of replicas dynamically anytime but you cannot change the number shards after-the-fact.

* By default, each index in Elasticsearch is allocated 5 primary shards and 1 replica

* Each Elasticsearch shard is a Lucene index

* There is a maximum number of documents you can have in a single Lucene index.

* As of LUCENE-5843, the limit is 2,147,483,519 (= Integer.MAX_VALUE - 128) documents.
