---
dg-publish: true
---
#definition #abstract-algebra/group-theory 

#### Definition
For a set $G$ and an [[Binary Operation|operation]] $\ast$ on $G$, we say $(G, \cdot)$ is a group if 
1) $\ast$ is associative on $G$. In other words, for $x,y,z \in G$, $x\ast (y\ast z) = (x \ast y) \ast z$.
2) $\ast$ has an identity element $e$ in $G$ ( $e \cdot g = g \cdot e = g$ ).
3) Every element in $G$ has an inverse in $G$ ( $g \cdot g^{-1} = g^{-1} \cdot g = e$ ).

#### Examples
1) $(\mathbb{Z}, +)$ is an [[Abelian Group|abelian]] group. 
2) $(\mathbb{R}^{\ast}, \cdot)$ is a group. 
3) $(GL_{n}(\mathbb{R}), \cdot)$ is a group (where $GL_n (\mathbb{R})$ is the set of invertible $n\times n$ matrices).

#### Notation Convention
For a general group, we say group $(G,\ast)$, identity element is $e$, and the inverse element of $g$ is $g^{-1}$ .

If the operation on $G$ is a multiplication operation, we say group $(G, \cdot)$, with identity element $e = 1$, and the inverse element of $g$ is $g^{-1}$.

If the operation on $G$ is an addition operation, we say group $(G, +)$, with identity element $e = 0$, and the inverse element of $g$ is $-g$.

#### Basic Properties of Groups
1) The inverse of any element is unique in a group.
