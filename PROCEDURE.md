# Procedure

`java -server -Xmx4g -jar blazegraph.jar`

Upload data and metadata

```sparql
SELECT *
WHERE {
    GRAPH ?g {?s ?p ?o}
}
```

`curl http://localhost:9999/blazegraph/namespace/um/sparql`

`./server.js --config=../blazegraph-config.json`

<https://um.es/data/LDD012546>
<http://localhost:8080/data/LDD012546>

`curl -H "Accept: text/turtle" http://localhost:8080/data/LDD012546`

`curl -H "Accept: application/ld+json" http://localhost:8080/data/LDD012546`

<http://localhost:8080/dataset/UMGenesDataset>

`curl -H "Accept: application/ld+json" http://localhost:8080/dataset/UMGenesDataset`

`service apache2 restart`

`ln -s /home/mikel/EHU-LSI/Docencia/2020-2021/MSc-UM/MSc-UM-2020-FAIR/LinkedDataServer/data/GenesUM.csv GenesUM.csv`
