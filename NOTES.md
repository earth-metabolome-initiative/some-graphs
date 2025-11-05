`curl -o VGF138_A02.ttl https://raw.githubusercontent.com/earth-metabolome-initiative/some-graphs/refs/heads/main/data/MSV000087728_VGF138_A02_merged_graph_f848f21ecaa2e577c55d5d084e2039f2.ttl`

`curl -o VGF138_A01.ttl https://raw.githubusercontent.com/earth-metabolome-initiative/some-graphs/refs/heads/main/data/MSV000087728_VGF138_A01_merged_graph_817b5714ccbe09fac5ad90813756f6bd.ttl`


Get info regarding a given node 

`rudof node --node "enpkg:V111819GP-01" VGF138_A02.ttl`

or 

`rudof node -n "enpkg:V111819GP-01" VGF138_A02.ttl`


We can directly fetch infor from the URL.

`rudof node -n "enpkg:V111819GP-01" https://raw.githubusercontent.com/earth-metabolome-initiative/some-graphs/refs/heads/main/data/MSV000087728_VGF138_A02_merged_graph_f848f21ecaa2e577c55d5d084e2039f2.ttl`

The following command parses the file VGF138_A02.ttl and shows its contents:

`rudof data VGF138_A02.ttl`

Its possible to merge multiple files while serielizing them to another format

`rudof data VGF138_A01.ttl VGF138_A02.ttl -r rdfxml -o output.rdf`

Visualize the graph using plntuml

`rudof data VGF138_A01.ttl -r plantuml -o VGF138_A01_graph.plantuml`

`rudof data VGF138_A02.ttl  -r plantuml -o VGF138_A02_graph.plantuml`

### Querying over SPARQL endpoint

`rudof query -q wikidata.sparql -e wikidata`


### ShEx