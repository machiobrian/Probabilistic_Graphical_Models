`Probabilistic Graphical Models`

PGM : is a techinique for compactly representing Joint Probabistic Distribution over random variables.
* It exploits conditional [independencies] btn variables.

Each graphical model is characterized by a graph that can be either:
* Directed
* Undirected (or both)
* A set of params associated with each graph.

`Graphical Models`
1. **Bayesian Models**
* Consists of a Directed Graph
* A conditional prob. distribution (CPD) (on each node) || Joint - all characteristics vs conditional - has a specific characteristics
* Each CPD is of the form **P(node|parent(node))**

2. **Markov Models**
* Consist of undirected graphs
* They are parameterized by factors - Factors represent how much 2 or more variables agree with each other.

### Bayesian Models / Networks
Mostly used when we want to represent a casual relationship btn the random variables.
> cardinality: the number of possible values a feature can assume

Joint Distribution over all the variables is just the product of all the CPDs in the network.




