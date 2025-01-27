#note #abstract-algebra 

What is [[Galois Theory]]?

#### Problem:

Write $\frac{1}{2+\sqrt{ 7 }}$ as $a+b\sqrt{ 7 }$ for $a,b \in \mathbb{Q}$.

*Solution:*
$$
\frac{1}{2+\sqrt{ 7 }} = \frac{{2-\sqrt{ 7 }}}{(2-\sqrt{ 7 })(2+\sqrt{ 7 })} = -\frac{2}{3} + \frac{1}{3} \sqrt{ 7 }.
$$

#### Definition:
$\mathbb{Q}[\sqrt{ 7 }] = \{ a+b\sqrt{ 7 } | a,b\in \mathbb{Q} \}$

*Observations:*
1) $\mathbb{Q} \subset \mathbb{Q}[\sqrt{ 7 }]$ (set $b=0$) so $0,1 \in \mathbb{Q}[\sqrt{ 7 }]$
2) $\mathbb{Q}[\sqrt{ 7 }]$ is stable under addition (and subtraction).
3) $\mathbb{Q}[\sqrt{ 7 }]$ is stable under multiplication.
4) $a,b\in \mathbb{Q}$ then $a+b\sqrt{ 7 }=0 \iff a=b=0$.
5) $\mathbb{Q}[\sqrt{ 7 }]$ is also stable (closed) under division by nonzero elements.

We will say that $\mathbb{Q}[\sqrt{ 7 }]$ is a *field*.

##### Proof of 4:

"$\implies$" is easy.

"$\impliedby$"

$a,b\in \mathbb{Q}$   $a+b\sqrt{ 7 }=0 \implies b\sqrt{ 7 }=-a \implies 7b^2=a^2$.

$\exists n \in \mathbb{N}$ with $n>0$ and $A=an, B=bn \in \mathbb{Z}$

$7b^2=a^2 \implies 7b^2n^2=a^2n^2 \implies 7(bn)^2=(an)^2 \implies 7B^2=A^2$, $A,B \in \mathbb{Z}$.

Set $d=\gcd(A,B)$ (only well defined if $A,B$ are not both 0, which is equivalent to $a,b$ not both $0$), so $A=d\bar{a}, B=d\bar{b}$, where $\bar{a},\bar{b} \in \mathbb{Z}$ and $\gcd(\bar{a},\bar{b})=1$.

$7(d\bar{b})^2=d\bar{a})^2 \implies 7d^2 \bar{b}^2 = d^2 \bar{a}^2 \implies 7\bar{b}^2 =\bar{a}^2 \implies 7 \mid \bar{a}^2 \implies 7 \mid \bar{a} \implies 7\bar{b}^2 =(7 \tilde{a})^2 \implies \dots$ *contradiction*


##### Observation:

$Q[\sqrt{ 7 }]$ is a [[Vector Space]] over $\mathbb{Q}$, it has basis $1,\sqrt{ 7 }$, so it has dimension $2$.


#### Conjugation:

Set $\varphi: \mathbb{Q}[\sqrt{ 7 }] \to \mathbb{Q}[\sqrt{ 7 }]$ 
$\varphi(a+b\sqrt{ 7 }) = a-b\sqrt{ 7 }$

##### Properties of $\varphi$:

1) $\varphi(0)= \varphi(0+0\sqrt{ 7 }) = 0-0\sqrt{7 }=0$.
2) $\varphi(1)= \varphi(1+0\sqrt{ 7 })=1-0\sqrt{ 7 }=1$.
	More generally, $\varphi(a)=a$ for all $a\in \mathbb{Q}$.
3) $\varphi$ preserves addition.
	$\varphi((a+b\sqrt{ 7 }) + (c+d\sqrt{ 7 }))=\varphi((a+c)+(b+d)\sqrt{ 7 }) = (a+c)-(b+d)\sqrt{ 7 }$ 
	$= (a-b\sqrt{ 7 })+(c-d\sqrt{ 7 }))= \varphi(a+b\sqrt{ 7 }) + \varphi(c+d\sqrt{ 7 })$.
4) $\varphi$ preserves multiplication.
5) $\varphi$ is a bijection.
	$\varphi^{-1} = \varphi$

$\varphi$ is an example of an [[Automorphism|automorphism]] of the field $\mathbb{Q}[\sqrt{ 7 }]$.

$\operatorname{id}_{\mathbb{Q}[\sqrt{ 7 }]}, \varphi$ are both automorphisms.

The set of all automorphisms of $\mathbb{Q}[\sqrt{ 7 }]$ is the [[Galois Group]] of $\mathbb{Q}[\sqrt{ 7 }]$.

$$
\{ \operatorname{id}_{Q[\sqrt{ 7 }]}, \varphi \} \subseteq \operatorname{Gal}({^{\textstyle \mathbb{Q}[\sqrt{ 7 }]}\big/_{\textstyle \mathbb{Q}}}).
$$
This inclusion is in fact an equality.

###### Proof:

Say $f:\mathbb{Q}[\sqrt{ 7 }] \to \mathbb{Q}[\sqrt{ 7 }]$ is an automorphism. Preserve $\mathbb{Q}$ ($f(a)=a \forall a\in \mathbb{Q}$), preserves addition and multiplication, and is a bijection.

We want that $f=\operatorname{id}_{\mathbb{Q}[\sqrt{ 7 }]}$ or $f=\varphi$.

Observe $f(\sqrt{ 7 }) \in \mathbb{Q}[\sqrt{ 7 }]$ uniquely determines $f$.
$f(\sqrt{ 7 })= u+v\sqrt{ 7 }$, $u,v \in \mathbb{Q}$.

$f(a+b\sqrt{7})=f(a)+f(b\sqrt{ 7 })=a+f(b)f(\sqrt{ 7 })$	$= a + (b)(u+v\sqrt{ 7 })=(a+bu)+(bv)\sqrt{ 7 }$
(this is from the fact that $f$ preserves addition and $f$ preserves $\mathbb{Q}$ and multiplication).

$(\sqrt{ 7 })^2 = 7 \implies (f(\sqrt{ 7 }))^2=f((\sqrt{ 7 })^2) = f(7)=7$
$\implies (f(\sqrt{ 7 }))^2 = 7$
$\implies f(\sqrt{ 7 }) = \pm \sqrt{ 7 }$

Thus $f(\sqrt{ 7 }) = \begin{cases}\sqrt{ 7 }, & f=\operatorname{id}_{Q[\sqrt{ 7 }]}\\ -\sqrt{ 7 }, & f=\varphi \end{cases}$, and these are the only two possibilities.

###### Application: 
Say $P(x)=x^n + c_{n-1}x^{n-1} + \ldots +c_{0}$, with $c_{i} \in \mathbb{Q} \forall 0 \leq i \leq n-1$.
If $P(x)$ has $a+b\sqrt{ 7 }$ as root, then $a-b\sqrt{ 7 }$ is also a root.

Say $\alpha = a+b\sqrt{ 7 }$ is a root of $P(x)$, then $\sum_{k=0}^{n}(c_{k}(\varphi(\alpha))^{k})=\varphi(P(\alpha))=\varphi(0)=0$, so $\sum_{k=0}^{n}(c_{k}(\alpha')^{k})=0$, $\alpha'$ is a root.

