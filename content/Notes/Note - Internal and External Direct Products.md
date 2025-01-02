---
dg-publish: true
---
#note #abstract-algebra/group-theory 
#### Question
What do we mean by "internal" direct product? What is an "external" direct product?

#### Recall
If $( G, \cdot )$, $( H, \ast )$, we can construct an (external) direct product $G \times H$ with component-wise operations. 
$$
(g,h) \otimes (g',h') = (g\cdot g', h\ast h').
$$

#### Theorem
Given groups $( G, \cdot )$, and $N,H \unlhd G$ that give an internal direct product decomposition of $G$, then
$$
f:H\times N \to G \text{ given by } f(h,n)=hn
$$
is an isomorphism.

#### Proof
$N,H \leq G$, $nh=hn\forall n\in N, h \in H$, $HN=G$.

$f$ is a morphism:
$$
f((h,n)\otimes (h',n')) \overset{?}{=} f(h,n)f(h',n')
$$
$f(h,n)=hn$, $f(h',n')=h'n'$, so $f(h,n)f(h',n')=hnh'n'=hh'nn'$.

$f$ is surjective: 
If $g\in G=HN \implies \exists h\in H, n\in N, g=hn=f(h,n) \implies f$ is onto.

$f$ is injective ($\iff \ker f = e_{{H\times N}}=(e_{H},e_{N})$)
$\ker f = \{  (h,n) \in H\times N :hn=f(h,n) = e_{G} \}$
$\implies h \in H, h= n^{-1}\in N \implies h\in H \cap N = \{  e_{G} \}$
$\implies h = n = \{  e_{G} \} \implies (h,n) = (e_{G},e_{G}) = (e_{H}, e_{N})$