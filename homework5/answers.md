## Planar Graphs

### 1. Redraw the graph with no edges cross

![8.7.2](./8.7.2.png)

### SOLUTION

![answer 1](a1.png)

---
### 2. Show the graph is not planar by finding a subgraph homeomorphic to either K5 or K3.3

![8.7.5](./8.7.5.png)

### SOLUTION

Let us try to find $K_{3,3}$ in the graph. We first note that the vertices a, c, and g each have degree 4. In $K_{3,3}$ each vertex has degree 3, so let us eliminate the edges (a, c) and (d, g) so that all vertices have a degree less or equal to 3. We note that edges (a, b) and (b, d) are in series, and edges (c, b) and (b, d) are in series too. Deleting the vertex b will obtain a $K_{3,3}$ bipartite graph by series reduction.
Therefore, the graph is not a planar graph.


![2.1](./2.1.png) 

---

### 3. Show that in any simple, connected, planar graph, $e \le 3v-6$.

### SOLUTION
A graph with only 1 vertex, and 0 edge does not satisfy the formula.
And a graph with 2 vertices, and 2 edges does not satisfy the formula either.

## Introduction to Trees
### 4. Give the Huffman code below

![9.1.15](./9.1.15.png)

(a) Decode the bit string $01111001001110$  
(b) Encode the word $LEADEN$

### SOLUTION
From the given Huffman code, we get the table
| Letter | Code  |
| :----: | :---- |
|   A    | 10    |
|   D    | 01111 |
|   E    | 00    |
|   L    | 01110 |
|   N    | 010   |
|   P    | 0110  |
|   S    | 11    |

(a) $01111001001110=DEANL$  
(b) $LEADEN=0111000100111100010$

---

### 5. Construct an optimal Huffman code for the set of letters in the table.
|    Letter     | Frequency |
| :-----------: | :-------: |
|   $\alpha$    |     5     |
|    $\beta$    |     6     |
|   $\gamma$    |     6     |
|   $\delta$    |    11     |
| $\varepsilon$ |    20     |
### SOLUTION
Repeatedly replacing the smallest 2 frequencies with the sum:

$$
\begin{aligned}
  5,6,6,11,20 &\rightarrow 5+6,6,11,20\\
  6,11,11,20 &\rightarrow 6+11,11,20\\
  11,17,20 &\rightarrow 11+17,20\\
  20,28
\end{aligned}
$$

Construct the tree working backward.

![9.1.24](./9.1.24.png)

---

### 6. Show that a tree is a planar graph

### SOLUTION
A connected tree is a graph with n vertices and n-1 edges, there is no cycle in a tree, so the face of a tree is always 1.  
Thus the tree satisfies Euler's formula $f=e-v+2$ where $f=1,\ e=v-1$

## Terminology and Characterization of Tree
### 7.

![9.2.8](./9.2.7-15.png)

(a) Find the children of d and of e.  
(b) Find the ancestors of c and of j.  
(c) Find the descendants of c and of e.  
(d) Find the terminal vertices.  
(e) Find the siblings of f and of h.

### SOLUTION
(a) The children of d are h and i, and the child of e is j.  
(b) The ancestors of c are a and b, and the ancestors of j are a, b, c, and e.  
(c) The descendants of c are e, f, g, and j, the descendant of e is j.  
(d) The terminal vertices are f, g, h, i, and j.  
(e) The siblings of f are e and g, and the sibling of h is i.

---

### 8. Draw a graph having the given properties or explain why no such graph exists.
(a) Tree; all vertices of degree 2  
(b) Acyclic; four edges, six vertices

### SOLUTION

(a) A tree with all vertices of degree 2 does not exist because all the terminal vertices of a tree have degree 1.  
(b)

![9.2.24](./9.2.24.png)

