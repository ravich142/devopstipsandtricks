- Elasticsearch’s cat shards API will tell you which shards are unassigned, and why
```bash
curl -XGET -s  localhost:9200/_cat/shards?h=index,shard,prirep,state,unassigned.reason| grep UNASSIGNED
```
