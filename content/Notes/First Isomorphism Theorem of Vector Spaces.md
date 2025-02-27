#theorem #abstract-algebra/vector-spaces

#### Intuition
This is exactly the analogue of [[Fundamental Isomorphism Theorem]] for groups, [[Fundamental Isomorphism Theorem (Ring)]] for rings, and every other first fundamental isomorphism theorem in algebraic theories.

#### Formal Statement
Let $T \in \mathscr{L}(V,W)$. Since $\operatorname{null}(T)$ is a subspace of $V$, we can define the quotient space ${^{\textstyle V}\big/_{\textstyle \operatorname{null}(T)}}$. Moreover,
$$
{^{\textstyle V}\big/_{\textstyle \operatorname{null}(T)}} \simeq \operatorname{range}(T) \subseteq W.
$$
#### Proof
We want to describe an isomorphism  $\tilde{T}:{^{\textstyle V}\big/_{\textstyle \operatorname{null}(T)}} \to \operatorname{range}(T)$.

Let us define $\tilde{T}(v + \operatorname{null}(T)) = Tv$, or the coset of $v$ with respect to $\operatorname{null}(T)$ maps to an element $Tv$ in $\operatorname{range}(T)$.

(Injectivity)
Assume $\tilde{T}(v + \operatorname{null}(T)) = 0$. Then by definition $Tv = 0 \implies v \in \operatorname{null}(T) \implies v - 0 \in \operatorname{null}(T) \implies v + \operatorname{null}(T) = 0 + \operatorname{null}(T) =$ zero of ${^{\textstyle V}\big/_{\textstyle \operatorname{null}(T)}}.$

(Surjectivity)
Since $\tilde{T}(v + \operatorname{null}(T)) = Tv$, it is obvious that $\operatorname{range}(\tilde{T}) = \operatorname{range}(T)$, so $\tilde{T}$ is surjective.

#### Corollaries