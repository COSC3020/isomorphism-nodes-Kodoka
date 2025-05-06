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

Let $G_1 = (V_1, E_1$ and $G_2 = (V_2, E_2)$ be two different graphs where the
number of nodes in the graphs, $n$, $= |V_1| \neq |V_2|$. $G_1$ and $G_2$ are
isomorphic if, and only if, there exists a bijection, $f$: $V_1 \implies V_2$.
