#theorem #abstract-algebra/vector-spaces

#### Intuition


#### Formal Statement
Consider a finite-dimensional vector space $V$, and $T\in \mathscr{L}(V,W)$. Then $\operatorname{range}T$ is a finite-dimensional subspace of $W$ and,
$$
\dim V =\dim (\operatorname{null}T) + \dim (\operatorname{range}T).
$$

#### Corollaries
1) If $V,W$ are finite-dimensional vector spaces with $\dim V > \dim W$, there exist no injective linear maps $T: V\to W$.
2) If $V,W$ are finite-dimensional vector spaces with $\dim V < \dim W$, there exist no surjective linear maps $T: V\to W$. 
3) A homogenous system with more variables than equations has non-trivial solutions.
4) A system with more equations than variables has no solution for some choice of constant terms.


#### Proof
*We want to show:*
5) $\operatorname{range}T$ is finite-dimensional.
6) $\dim$ add correctly, so we need bases for $V$, $\operatorname{null}T$, $\operatorname{range}T$.

Since $\operatorname{null}T$ is a subspace of a finite-dimensional vector space $V$, $\operatorname{null}T$ is finite-dimensional.Let $\dim \operatorname{null}T = m \leq \dim V$, and let $u_{1},\ldots, u_{m}$ be a basis of $\operatorname{null}T$. Thus, $u_{1},\ldots,u_{m}$ is a linearly independent list in $V$, which is finite-dimensional, so $u_{1}, \ldots, u_{m}$ can be extended to a basis of $V$:
$$
u_{1},\ldots,u_{m},v_{1},\ldots,v_{n}.
$$
Thus, $\dim V = m+n$. To finish the proof, we claim $Tv_{1},\ldots, Tv_{n}$ is a basis of $\operatorname{range}T$:

Let $v\in V$. Then,
$$
v=a_{1}u_{1}+\cdots + a_{m}u_{m}+ b_{1}v_{1}+\cdots + b_{n}v_{n}.
$$
Apply $T$ to both,
$$
Tv=0+\cdots + 0 + b_{1}Tv_{1}+ \cdots + b_{n}Tv_{n},
$$
So $Tv_{i}$ span $\operatorname{range}T$.

Now we show that $Tv_{1}, \ldots, Tv_{n}$ is linearly independent. Suppose $c_{1},\ldots,c_{n} \in \mathbb{F}$ and $c_{1}Tv_{1} + \cdots + c_{n}Tv_{n} = 0$, so $T(c_{1}v_{1} + \cdots + c_{n}v_{n})=0$, or equivalently $c_{1}v_{1}+\cdots + c_{n}v_{n} \in \operatorname{null}T$. Hence $c_{1}v_{1}+ \cdots + c_{n}v_{n}= d_{1}u_{1}+ \cdots + d_{m}u_{m}$ since $u_{i}$'s are a basis of $\operatorname{null}T$. Since $u$'s + $v$'s are a basis of $V_{1}$, they are linearly independent, so there exist no non-trivial linear combination of $u$'s and $v$'s equal to $0$. Therefore, $Tv_{1} , \ldots, Tv_{n}$ are linearly independent. $\qquad \qquad \square$
