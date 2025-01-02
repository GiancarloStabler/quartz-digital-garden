---
dg-publish: true
---
#note  #abstract-algebra/group-theory 

For a [[Group|group]] $( G, \cdot )$, with [[Normal Subgroup|normal subgroup]] $N \unlhd G$, there is a [[Group Homomorphism|morphism]] $\pi:G\to {G}/{N}$ where $\pi(g)=gN$. We also have $\pi$ is a surjective morphism with [[Kernel|kernel]] equal to $N$.

#### Question: How do subgroups of $G$, $G/N$ relate?

Let $H \leq G$, $N \leq H$.

$\pi(H) = \{ \pi(h) : h\in H \} = \{ hN : h\in H \}$
$hN = \{  hn : n\in N \} \subseteq H$
$N \leq H$

$hN \in H/N \leftarrow N \unlhd H$
$H/N \subseteq G/N$ (<- can see this)

Claim: $H/N \leq G/N$
e.g. check stable under products:

$hN,h'N \in H/N \subseteq G/N \implies$
$hN \cdot h'N = (hh') N \in H/N$ (<- $\cdot$ is the product in $G/N$)

Recall: If $Q \leq G/N$, then $\pi^{-1} Q = \{  g\in G : \pi(g) \in Q \}$

Lemma: $N \leq \pi^{-1} Q \leq G$

Proof: ...

Lemma: $Q = \pi^{-1}Q/N$

Proof: 
If $gN \in Q$ then $gN = \pi(g)$ so $g\in \pi^{-1}Q$. Thus $gN \in \pi^{-1}Q/N$, so $Q \subseteq \pi^{-1}Q/N$.
If $gN\in G/N$ and $gN \in \pi^{-1}Q/N$, then $gN = g'N$ for some $g'\in \pi^{-1}Q$. We have $g'N = \pi(g') \in Q$. Therefore, $gN = g'N \in Q$, so $\pi^{-1}Q/N \subseteq Q$

### The Correspondence Theorem
We have a one-to-one correspondence between subgroups of $G/N$ and subgroups of $G$ that contain $N$. 
$N \leq H \leq G\quad \rightarrow \quad H/N$
$N \leq \pi^{-1}Q \leq G\quad \leftarrow \quad Q \leq G/N$

##### Proof 
It remains to prove that if $N\leq H \leq G \implies \pi^{-1}(H/N) = H$.

Let $h\in H$, so $\pi(h) = hN \in H/N$. We have that $h\in \pi^{-1}(H/N)$. Let $g\in \pi^{-1}(H/N) \implies gN = \pi(g) \in H/N \implies \exists h \in H, g\in gN = hN \implies g\in hN \implies g - h\cdot n$ for some $n \in N \implies g \in H. \qquad \square$

##### Remark
Correspondences above preserve inclusions and normality. (Proofs omitted but are supposedly easy).

##### Question
If $f:G\to F$ is a morphism, then $f(G) \leq F$. In particular, if $H\leq G \implies f(H) \leq F$.

If $N\unlhd G$, $\pi:G\to G/N$. Assume $H\leq G$ does not contain $N$. This implies $\pi(H) \leq G/N$. Which subgroup of $G/N$? 

##### Answer:
$\pi(H) = HN/N$.

$HN - \{  hn :h\in H, n \in N \}$
$HN \leq G$
$N \unlhd H$

##### Proof
If $h\in H \subseteq G \implies \pi(h) = hN \in HN/N$, $h\in HN$ and $N \unlhd HN$. Therefore, $\pi(H) \subseteq HN/N$.

Conversely, if $gN \in HN/N$ ($gN = h\cdot nN = hN$) for some $h\in H, n\in N$, $gN = hN = \pi(h) \implies gN \in \pi(H). \qquad \square$

##### Example
$G=\mathbb{Z}$, $N=100\mathbb{Z}$, $H=40\mathbb{Z}$ 

What is the image of $H$ in $G/N = \mathbb{Z}_{100}$?

*Solution 1:* $H=\langle 40 \rangle \leq \mathbb{Z} \implies$
$$
\begin{align*}
\pi(H) &=\langle \pi(40) \rangle, \\
&= \langle 40 \rangle \leq \mathbb{Z}_{100},\\
&= \langle \gcd(40,100) \rangle,\\
&= \langle 20 \rangle.
\end{align*}
$$

