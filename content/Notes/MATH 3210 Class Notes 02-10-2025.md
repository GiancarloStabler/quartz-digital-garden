#note #abstract-algebra/vector-spaces 

#### Recall [[Linear Map|Linear Maps]]

#### Lemma
Suppose $v_{1},\ldots, v_{n}$ is a basis of $V$ and $w_{1},\ldots, w_{n} \in W$. Then there exists a unique linear map $T: V \to W$ such that,
$$
Tv_{k} = w_{k} \quad \forall k=1,\ldots, n.
$$
##### Proof
All $v\in V$ can be written uniquely as $v=c_{1}v_{1} + \ldots + c_{n}v_{n}$. Define $T(c_{1}v_{1}+ \ldots + c_{n}v_{n}) = c_{1}w_{1}+\ldots + c_{n}w_{n}$...

#### Defined [[Algebra on the Set of Linear Maps]]

##### Definition
If $T \in \mathscr{L}(V,W)$ and $S \in \mathscr{L}(W,U)$, then the product $ST \in \mathscr{L}(V,U)$ is given by,
$$
(ST)(v)=S(Tv).
$$

#### Proposition
Assume all products "make sense".
1) (Associativity) $(T_{1}T_{2})T_{3}=T_{1}(T_{2}T_{3})$.
2) (Identity) $TI_{V}=I_{W}T=T$
3) (Distributivity) $(S_{1}+S_{2})T = S_{1}T + S_{2}T$, and $S(T_{1}+T_{2})= ST_{1}+ST_{2}$.

Note: $ST \neq TS$.

A good example of this would be the "differentiation" and "multiplication by $x^6$" maps in the algebra of linear maps from $P(\mathbb{R})$ to itself. They very much so do not commute under composition.

#### Defined [[Nullspace]]

#### For the Exam
- True/false conceptual questions.
- Some computational problems (find the nullspace of a given map, determine a vector that is linearly independent with some set of vectors, etc.)
- Some uniqueness proof (prove that the additive inverse is unique in a general vector space, etc.)
- If it goes terribly it will likely be curved/adjusted.