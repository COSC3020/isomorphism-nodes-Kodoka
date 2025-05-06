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
  
As such, one way or another, if $|V_1| \neq |V_2|$, there can be no function $f:
V_1 \implies V_2$ that can be both injective and surjective.  

Thus, as an isomorphism between $G_1$ and $G_2$ must have a bijection, $f: V_1
implies V_2$, and no bijection like that can exist when $|V_1| \neq |V_2|$, if
$|V_1| \neq |V_2|$, then $G_1$ and $G_2$ cannot be isomorphic.  

## Sources

I used my work on the isomorphism-nodes-connectivity exercise, to help me put
together this proof:  

https://github.com/COSC3020/isomorphism-nodes-connectivity-Kodoka  

## Plagiarism Notice

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
