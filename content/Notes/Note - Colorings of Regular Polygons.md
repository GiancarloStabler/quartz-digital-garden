---
dg-publish: true
---
#note #abstract-algebra/group-theory  

#### Definition
$P_{n}$ is a regular $n$-gon. If $P_{n}$ is labeled, the vertices are labeled $1,2,\ldots, n-1$.

#### Definition
A labeled coloring of $P_{n}$ with blue and red is an assignment of a color (blue or red) to each label.

There are $2^n$ labeled colorings: two independent choices for each of $n$ labels.

#### Definition
An (unlabeled) coloring removes labels from a labeled coloring. 

Two unlabeled colorings are considered the same if they come from labeled colorings that differ by a rigid motion, an element of $D_{n}$.

An unlabeled coloring is an [[Orbit (group)|orbit]] of $D_{n}$ acting on labeled colorings.

##### Example ($n=3$)
$2^3=8$ labeled colorings 

And we have 4 different unlabeled colorings.
*Ignore this TikZ diagram*
```tikz
\usepackage{circuitikz}

\begin{document}
\begin{circuitikz}
\tikzstyle{every node}=[font=\LARGE]
\draw [short] (2.5,11.5) -- (4.75,15.25);
\draw [short] (4.75,15.25) -- (6.75,11.5);
\draw [short] (2.5,11.5) -- (6.75,11.5);
\node [font=\LARGE] at (4.75,15.75) {1};
\node [font=\LARGE] at (7.25,11.25) {2};
\node [font=\LARGE] at (2,11.25) {3};
\draw [ fill={rgb,255:red,56; green,142; blue,255} ] (4.75,15.25) circle (0.25cm);
\draw [ fill={rgb,255:red,56; green,142; blue,255} ] (2.5,11.5) circle (0.25cm);
\draw [ fill={rgb,255:red,56; green,142; blue,255} ] (6.75,11.5) circle (0.25cm);
\end{circuitikz}
\end{document}
```


#### Recall
$G$ group, $X$ set. A group action of $G$ on $X$ is an association $\forall g\in G, \forall x \in X$ have $g\bullet x \in X$ (the action of $g$ on $x$) such that 
$$
\begin{cases}
e_{G} \bullet x = x & \forall x\in X \\
g\bullet (g' \bullet x) = (gg') \bullet x & \forall x\in X \forall g,g'\in G 
\end{cases}
$$
For $x\in X$, $\operatorname{orb}(x) = \{  g\bullet x : g\in G \}$.

[[Orbit (Group)]]
[[Stabilizer (Group)]]
#### Theorem (Burnside Theorem)
The number of distinct unlabeled colorings is equal to the number of distinct orbits, which can be described as,
$$
\# \text{ distinct orbits } = \frac{1}{|G|} \sum_{g\in G}^{} |\operatorname{fix}_{x} (g)|
$$

##### Example ($n=3$)
$2^3=8$ labeled colorings.

$D_{3} = \{  e, \sigma, \sigma^2, \tau, \sigma \tau,\sigma^2\tau \}$

$\operatorname{fix}(e) = X$, 8 labeled colorings.
$\operatorname{fix}(\sigma) =$ the fully red, and fully blue colorings.
$\operatorname{fix}(\sigma^2) =$ again the same 2 fully red, and fully blue colorings.
$\operatorname{fix}(\tau)=$ RRR, BBB, RBB, BRR colorings (R=red, B=blue, order is clockwise from top vertex of triangle)
$\operatorname{fix}(\sigma \tau) =$ again 4 labeled colorings
$\operatorname{fix}(\sigma^2\tau) =$ again 4 labeled colorings

Applying Burnside theorem,
$\# \text{ orbits } = \frac{1}{6}\left( 8+2+2+4+4+4\right)=\frac{24}{6}=4$ 

Thus there are 4 unlabeled colorings.


##### Example ($n=4$)
Let us count fixed labeled colorings for each $g\in D_{4}$.

$D_{4}=\{ e,\sigma,\sigma^2,\sigma^3,\tau,\sigma \tau,\sigma^2\tau,\sigma^3\tau \}$

$\operatorname{fix}(e) =$ all $16=2^4$ labeled colorings.
$\operatorname{fix}(\sigma)=$ $2$ colorings: RRRR, BBBB.
$\operatorname{fix}(\sigma^3)=$ $2$ colorings: RRRR, BBBB.
$\operatorname{fix}(\sigma^2)=$ $4$ colorings: RRRR, BBBB, RBRB, BRBR.
Take $\tau$ as a reflection across one of two diagonals:
$\operatorname{fix}(\tau)=$ $8$ colorings: RRRR, BBBB, RBRR, BRBB, RRRB, BBBR, RBRB, BRBR.
Take $\tau$ as a reflection across the horizontal:
$\operatorname{fix}(\tau)=$ $4$ colorings: RRRR, BBBB, RRBB, BBRR.
Take $\tau$ as reflection across vertical:
$\operatorname{fix}(\tau)=$ $4$ colorings: RRRR, BBBB, RBBR, BRRB.

$\#$ unlabeled colorings $=$ $\#$ orbits $= \frac{1}{8}(16+2+2+4+8+8+4+4)= 6$.

##### Example ($n=5$)
$D_{5}=\{ e,\sigma,\sigma^2,\sigma^3,\sigma^4, \tau,\sigma \tau,\sigma^2\tau,\sigma^3\tau,\sigma^4\tau \}$

$\operatorname{fix}(e) =$ all $32=2^5$ labeled colorings.
Take $\sigma$ as any non-trivial rotation:
$\operatorname{fix}(\sigma)=$ $2$ colorings: RRRR, BBBB.
Take $\tau$ any reflection:
$\operatorname{fix}(\tau)=$ $8$ colorings: "opposing" vertices have same color, $2\cdot 2 \cdot 2 = 8$.

$\#$ unlabeled colorings $= \#$ orbits $= \frac{1}{10}(32+4\cdot 2 + 5 \cdot 8) = 8$ distinct unlabeled colorings.

#### Remark
$S_{4}$ acts similarly on a regular tetrahedron, so we can use it to count the number of unlabeled colorings on that.

[[Proof of Burnside's Theorem]]