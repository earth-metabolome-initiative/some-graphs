`curl -o simple.ttl https://raw.githubusercontent.com/earth-metabolome-initiative/some-graphs/refs/heads/main/data/MSV000087728_VGF138_A02_merged_graph_f848f21ecaa2e577c55d5d084e2039f2.ttl`

Get info regarding a given node 

`rudof node --node "enpkg:V111819GP-01" simple.ttl`

or 

`rudof node -n "enpkg:V111819GP-01" simple.ttl`


We can directly fetch infor from the URL.

`rudof node -n "enpkg:V111819GP-01" https://raw.githubusercontent.com/earth-metabolome-initiative/some-graphs/refs/heads/main/data/MSV000087728_VGF138_A02_merged_graph_f848f21ecaa2e577c55d5d084e2039f2.ttl`

The following command parses the file simple.ttl and shows its contents:

`rudof data simple.ttl`