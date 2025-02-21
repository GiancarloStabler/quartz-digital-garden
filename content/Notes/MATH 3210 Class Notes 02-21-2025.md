#note #abstract-algebra/vector-spaces 

### Invertibility and Isomorphisms
#### Defined [[Inverse (Linear Map)]]

#### Theorem
An invertible [[linear map]] has a unique inverse.
#### Notation
If $T \in \mathscr{L}(V,W)$ is [[Inverse (Linear Map)|invertible]], let $T ^{-1} \in \mathscr{L}(W,V)$ denote the inverse of $T$. 

#### Theorem
A linear map $T$ is invertible if and only if it is injective and surjective.

##### Proof
("$\implies$")
Assume $T \in \mathscr{L}(V,W)$ is invertible. Suppose $u,v \in V$ and $Tu =Tv$.
$$
\begin{align*}
Tu = Tv & \implies T ^{-1}(Tu) = T^{-1}(Tv) \\
& \implies Iu = Iv \\
& \implies u=v \implies \text{ injective}.
\end{align*}
$$
Let $w \in W$. Then,
$$
\begin{align*}
w = Iw &= (TT^{-1})w \\
&= T (T^{-1} w) \in V \implies \text{ surjective}.
\end{align*}
$$
("$\impliedby$")
Assume $T$ is injective and surjective. For each $w \in W$, let $S(w) \in V$ be the unique element of $V$, such that $T(S(w)) = w$. This is guaranteed to exist and be unique since $T$ is injective and surjective. Thus, $TS =I_{w}$. Also, let $v \in V$, then $T(ST(v)) = (TS)(Tv) = I_{w}(Tv) = Tv$. Therefore, since $T$ is injective, $v = STv$, so $ST = I_{v}$.

Finally, we must show that $S$ is a linear map. Let $w_{1},w_{2}\in W$ and $\lambda \in \mathbb{F}$, then $T(S(w_{1})+S(w_{2})) = TS w_{1} + TS w_{2} = w_{1} + w_{2}$. Thus, $Sw_{1}+ Sw_{2}$ is the unique element of $V$ which maps to $w_{1}+w_{2}$ under $T$. Therefore, $S(w_{1}+w_{2}) = S(w_{1})+S(w_{2})$ by definition.

#### Question
Is injectivity alone (or surjectivity alone) enough to have invertibility of a linear map $T \in \mathscr{L}(V)$?

##### Answer
No, if $V$ is infinite-dimensional; yes, if $V$ is [[Finite-Dimensional|finite-dimensional]].

