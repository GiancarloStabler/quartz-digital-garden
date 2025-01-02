---
dg-publish: true
---
#definition #abstract-algebra/group-theory 

#### Definition
[[Group]] $( G, \cdot )$, $N,H \unlhd G$. 
Assume:
	$N \cap H=\{ e_{G} \}$
	$HN = G$ and $hn=nh$ for all $n\in N, h \in H$.
Then we say $N,H$ give an internal direct product decomposition of $G$.

#### Examples
1) $N = \{ e_{G} \},H=G \unlhd ( G, \cdot )$
	$N\cap H = \{ e_{g} \}$
	$HN = G \cdot e_{G} = G$
	$\implies \{ e_{G} \}$ and $G$ give internal direct product decomposition of $G$. 
2) $G=( \mathbb{Z}_{6}, + )$
	$N=\langle 2 \rangle=\{ 0,2,4 \}$
	$H=\langle 3 \rangle=\{ 0,3 \}$
	$N \cap H = \{ 0 \}$
	$'HN' = H + N = \{ 0,3,2,5=3+2,4,7=1=3+4 \} = \mathbb{Z}_{6}=G$
	$\implies$ $N$ and $H$ give internal direct product decomposition of $\mathbb{Z}_{6}$.

#### Non-Examples
1) $G=( \mathbb{Z}, + )$
	$N=\langle 2 \rangle, H=\langle 3 \rangle$
	$H+N = \mathbb{Z}:H+N\leq \mathbb{Z}$
	The generator of $\mathbb{Z}$, $1$, is in $H+N$, but the $H\cap N \neq 0$.
2) $G=D_{3}$
	$H=\langle \tau \rangle, N=\langle \sigma \rangle$
	$H\cap N=\{ e \}$
	$HN=D_{3}$
	But $H$ is not normal, so $H$ and $N$ do not give internal direct product decomposition.

#### See
- [[Note - Internal and External Direct Products]]
