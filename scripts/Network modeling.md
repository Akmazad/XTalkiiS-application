### Data
#### First Data matrix
- sample: see the data directory
- Is a data matrix. 
- Could be from organism **A**. 
- This includes Gene Symbols.

#### Second Data matrix
- sample: see the data directory
- Is a data matrix. 
- Could be from organism **B**. 
- This includes Gene Symbols.

### Network modeling
#### Type
- Bipartite network: genes from A connects with genes from B (Inter-species network). 
- Complete network: genes from A connects with genes from B (Inter-species network) and genes in A connects with each others, likewise genes in B (Intra-species network). . 
#### Method
- Correlation (undirected network): the edges could be modeled based on all pair-wise correlations among expression vectors, followed by a threshold (could be preset or inferred). Python or R package could be available to compute the correlations.
- Causal network: the edges could be modeled via some graphical models (e.g. Bayesian network) based on the expression vectors. R-package called `bnlearn` has a bunch of methods implemented for this.
- Deep learning based approach
- Probabilistic modeling of "A" network, that is initially data-driven (Exponential random graph model[https://socialabstractions-blog.tumblr.com/post/53391947460/exponential-random-graph-models-in-python])
