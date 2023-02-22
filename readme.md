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

`Bayesian Models / Networks`

Mostly used when we want to represent a casual relationship btn the random variables.
> cardinality: the number of possible values a feature can assume

Joint Distribution over all the variables is just the product of all the CPDs in the network.

`Hidden Markov Model`
* A graphical model used to predict hidden states
* Uses sequential data: text, speech etc.
~~~~
            Fundamental factor about the HMM: Markov Property
The future states/events only rely on the current state/event.

            First Order Markov Model:
P(s(t)|s(t-1)) : Probability of state t is only dependent on state t-1

As the order increases the number of past dependancies also increases:

            Second Order Markov Model
P[s(t)|s(t-1),s(t-2)] ; prob. of state 2 is dependent on states t-1 & t-2

Eventually the idea is to model the joint probability:
Such that the prob. of S(t) = {s1,s2,s3} - We make use of the joint condition probability rule.
~~~~

`Transition Probability:`
* The probability of one state changing with respect to another.
Defined by an (M x M) matrix
* When the machine transitions from one state to another, the sum f all tranistion probabilities given the current state should be = 1.

`Inintial Probability Distribution`
* The machine has to start from a state. The initial state of Markov Model when t=0.

`Emission Probability Matrix`
* States are Hidden
* However, there are Visible/Observable **Symbols** as the states change.
* With every observable symbol: there is a probability of emitting a symbol.

`Attributes/Properties of HMM`
~~~~
1. States
2. Transition prob matrix [M x M]
3. Initial Probability Distribution (pi)
4. Markov Chain : (Fully observable & autonomous)
5. Final/Absorbing State
    - Observable/visible Symbol
6. Emission Prob Matrix 
~~~~


