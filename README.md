# Isomorphism

Prove that if two graphs $A$ and $B$ have the same number of nodes and are
completely connected, they must be isomorphic. I have started with the formal
definition of isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

If we have two completely connected graphs with the same number of vertices, then any bijection between their vertex sets will preserve adjacency. Since every vertex is connected to every other vertex, no matter how we map the vertices, the edges will map correctly, and the graphs will be isomorphic.

Pt1:
This portion of the proof tells us that two graphs having the same number of nodes atleast doesnt discount their ability to be Isomorphic.

$V_1 <= V_2$ and $V_2 <= V_1$ needs to be true for the graph to be both 1-1 and Onto meaning:

let:
num_v_in_G1 = $G_1$.numVerticies()
num_v_in_G2 = $G_2$.numVerticies()

= num_v_in_G1 <= num_v_in_G2 & num_v_in_G1 >= num_v_in_G2

= num_v_in_G1 == num_v_in_G2

so we can understand that only when the number of verticies in both graphs are equal do we satisfy the one-to-one and onto part of the isomorphic graph definition. 

Pt2:
$G_1$ and $G_2$ are complete graphs, this means that every pair of verticies in $G_1$ is connected by an edge. so for any  $u,v \in V_1$, the edge $(u, v) \in E_1$ Since $f$ is bijective, f(u) and f(v) in $G_2$ are also connected by an edge. since this holdes for all pairs of verticies in $G_1$ we can infer that $G_2$ is also a complete graph.

and so $G_1$ and $G_2$ are isomorphic because each node in both graphs are connected to every other node in the graphs.

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.