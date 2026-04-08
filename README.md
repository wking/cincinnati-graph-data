Following [this process][OTA-520], the graph is hosted at https://raw.githubusercontent.com/wking/cincinnati-graph-data/demo/cincinnati-graph.json , and we can set the cluster up to consume with:

```console
$ oc patch clusterversion version --type json -p '[{"op": "add", "path": "/spec/upstream", "value": "https://raw.githubusercontent.com/wking/cincinnati-graph-data/demo/cincinnati-graph.json"}]'
```

[OTA-520]: https://redhat.atlassian.net/browse/OTA-520
