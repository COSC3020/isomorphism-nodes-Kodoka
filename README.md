# Isomorphism

Prove that if two graphs $A$ and $B$ do not have the same number of nodes, they
cannot be isomorphic. I have started with the formal definition of isomorphism
below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

## My Proof

Let $G_1 = (V_1, E_1)$ and $G_2 = (V_2, E_2)$ be two different graphs where the
number of nodes in the graphs, $|V_1| \neq |V_2|$. $G_1$ and $G_2$ are isomorphic
if, and only if, there exists a bijection, $f: V_1 \implies V_2$. That is to
say for all $u, v \in V_1: (u, v) \in E_1 \Longleftrightarrow (f(u), f(v)) \in E_2$.  

Such a bijection requires equivalent cardinality between $V_1$ and $V_2$ as:
* Creating an injective mapping from $V_1$ into $V_2$ cannot exist if $|V_1| >
  |V_2|$, because, via the pigeonhole principle, at least two verticies within
  $V_1$ would have to be mapped onto a single vertex within $V_2$.
* Creating a surjective mapping from $V_1$ into $V_2$ cannot exist if $|V_1| <
  |V_2|$, because some vertex in $V_2$ would have no vertex within $V_1$ to
  map from.
Thus, one way or another, if $|V_1| \neq |V_2|$, there can be no function $f:
V_1 \implies V_2$ that can be both injective and surjective.
