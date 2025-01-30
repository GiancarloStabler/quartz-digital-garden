#definition #abstract-algebra/ring-theory 

#### Definition
For rings $(R, +, \cdot)$ and $(S, +, \cdot)$, $f: (R,+, \cdot) \to (S, +, \cdot)$ is a morphism if,
1) $f(r+r')= f(r) + f(r')$ for all $r,r' \in R$.
2) $f(r \cdot r') = f(r) \cdot f(r')$ for all $r,r' \in R$.

Additionally, 
- If $R,S$ are unital ring, we say $f$ is a morphism of unital rings if additionally $f(1_{R})=1_{S}$.
- If $f$ is a bijective morphism, say $f$ is an isomorphism.
- If there exists an isomorphism $f:R \to S$, say $R \simeq S$.
- If $f: R \to R$ is an isomorphism, say $f$ is an automorphism.

#### Properties
- $f(-x)=-f(x)$
- $f(n_{\mathbb{Z}}\cdot x)=n_{\mathbb{Z}}\cdot f(x)$ for all $n \in \mathbb{Z}$.
- $f(x^n)=(f(x))^n$ for all $n \geq 1$.
- If $x$ is invertible for multiplication (in a unital ring), then there exists $y=x ^{-1}$, such that $yx=xy=1_{R}$, and $f$ is a morphism of unital rings, then $f(x)$ invertible, $(f(x)) ^{-1} = f(x ^{-1})$.


#### Examples


