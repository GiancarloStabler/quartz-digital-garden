---
dg-publish: true
---
#note #number-theory/pells-equation
#### General Pell's Equation
$$
x^2-dy^2=1 \text{ for } d\in \mathbb{Z}^{+}, d\not = \square.
$$

#### Recall 
Units in $\mathbb{Z}[\sqrt{ d }]$ are $x+y\sqrt{ d }$ where $x^2-dy^2=\pm 1$.

#### Theorem (Lagrange)
For all $d\in \mathbb{Z}^+, d\\not = \square$, $x^2-dy^2=1$ has a solution in $\mathbb{Z}^+$.

#### Solving Specific Pell's Equations

##### Example
Find all positive integral solutions to $x^2-7y^2=1$.
	$x^2=7y^2+1$ and compute right hand side at $y=1,2,\ldots$ until it's a square.

$7(1)^2+1=8 \not = \square$
$7(2)^2+1=29 \not= \square$
$7(3)^2+1=64=8^2$

So we have a solution: $x=8,y=3$.

Then, since $N(8+3\sqrt{ 7 })=1$, $N((8+3\sqrt{ 7 })^n)=1$ and we can find infinitely many integral solutions of this form.

In fact, solutions of this form make up *all* integral solutions to this equation (up to sign on each value). 
#### Lemma
For $d\in \mathbb{Z}^+, d\not = \square$ there are infinitely many $x,y\in \mathbb{Z}^+$ such that $|x-y\sqrt{ d }|< \frac{1}{y}$ ($|\frac{x}{y}-\sqrt{ d }| < \frac{1}{y^2}$)

##### Example
$\sqrt{ 2 }=1.414\dots \approx \frac{14}{10} \approx \frac{141}{100}$
	$| \frac{7}{5}-\sqrt{ 2 }|=0.014\dots< \frac{1}{5^2}=0.04$
	$| \frac{141}{100}-\sqrt{ 2 }| = 0.004\dots < \frac{1}{100^2}=\frac{1}{10^4}=0.0001$

##### Proof
Pick $m>1$ in $\mathbb{Z}$. Look at $m+1$ numbers $0,\sqrt{ d }, 2\sqrt{ d },\ldots, m\sqrt{ d }$ and their decimal (fractional) parts in $[0,1)$.

$k\sqrt{ d }= a_{k}+ \varepsilon_{k}$ with $a_{k}\in \mathbb{Z}, a_{k} \geq 0$, and $0\leq \varepsilon_{k} \leq 1$.

Break up $[0,1)$ into the $m$ intervals $[ 0, \frac{1}{m})$, $[\frac{1}{m}, \frac{2}{m})$, $\ldots$, $[\frac{{m-1}}{m},1)$.

The $m+1$ numbers $\varepsilon_{0}, \varepsilon_{1}, \varepsilon_{2},\ldots, \varepsilon_{m}$ in $[0,1)$ lie in these $m$ intervals so the [[pigeonhole principle]] implies that some $\varepsilon_{k},\varepsilon_{\ell}$ in the *same* $[\frac{j}{m}, \frac{j+1}{m})$ for some $j=0,1,\ldots,m-1$. Without loss of generality, $k > \ell$.

$k\sqrt{ d }-a_{k} = \varepsilon_{k}$ and $\ell \sqrt{ d }-a_{\ell}=\varepsilon_{\ell}$ are in $[\frac{j}{m}, \frac{j+1}{m})$, so $0 \leq |\varepsilon_{k}-\varepsilon_{\ell}| < \frac{1}{m}$.

$$
\begin{align*}
0 \leq |k\sqrt{ d }-a_{k} - (\ell \sqrt{ d }-a_{\ell})| &< \frac{1}{m}\\
0 \leq |(k-\ell)\sqrt{ d }-(a_{k}-\ell_{k})| &< \frac{1}{m}\\
0 \leq |\underset{x}{(a_{\ell}-a_{k})} + \underset{y\in \mathbb{Z}^+}{(k-\ell)}\sqrt{ d }| &< \frac{1}{m}\\
|x-y\sqrt{ d }| &< \frac{1}{m}
\end{align*}
$$

$0 \leq \ell < k \leq m \implies y=k-\ell <m \implies \frac{1}{m} < \frac{1}{y}$, so $|x-y\sqrt{ d }| < \frac{1}{m} < \frac{1}{y}$.

$|x-y\sqrt{ d }|< \frac{1}{y}, y\in \mathbb{Z}^+$

$$
\begin{align*}
\implies |x-y\sqrt{ d }| < 1 \implies x &> y\sqrt{ d }-1\\
&\geq \sqrt{ d }-1\\
&\geq \sqrt{ 2 }-1\\
&> 0 \implies x\in \mathbb{Z}^+.
\end{align*}
$$
For each $m\in \mathbb{Z}^+$ we found an $x,y \in \mathbb{Z}^+$ such that $y < m$ and $|x-y\sqrt{ d }|< \frac{1}{m} < \frac{1}{y}$.

Note $|x-y\sqrt{ d }| > 0$ since $\sqrt{ d } \not \in \mathbb{Q}$.
Pick  $m'\in \mathbb{Z}^+$ such that $\frac{1}{m'} < |x-y\sqrt{ d }|$. Apply argument to get $|x'-y'\sqrt{ d }| < \frac{1}{m'}, y' < m' < \frac{1}{y'}$, etc, etc. $\quad \square$

##### Remark
Try solving $x^2-61y^2 = 1$ by $x^2=61y^2+1$ and $y=1,2,3,\ldots$ . Good luck...

#### Claim
We know by lemma that $|x-y\sqrt{ d }| < \frac{1}{y}$ infinitely often in $\mathbb{Z}^+$.

*Claim:* $|x-y\sqrt{ d }| < \frac{1}{y} \implies |x^2-dy^2| < 2\sqrt{ d }+1$.
$x=x-y\sqrt{ d }+ y\sqrt{ d }\leq |x-y\sqrt{ d }|+y\sqrt{ d } < \frac{1}{y}+y\sqrt{ d }\leq 1+y\sqrt{ d }$. Also see $x\leq y\sqrt{ d }+1$ by picture in proof of the lemma (still don't have a good way to do diagrams...black box this I guess).

So
$$
\begin{align*}
|x^2-dy^2| &= |(x+y\sqrt{ d })(x-y\sqrt{ d }) )|\\
&= |x+y\sqrt{ d }||x-y\sqrt{ d }|\\
&= (x+y\sqrt{ d })|x-y\sqrt{ d }|\\
&= (x+y\sqrt{ d }) \frac{1}{y}\\
& \leq (1+y\sqrt{ d } +y\sqrt{ d }) \frac{1}{y} = (1+2y\sqrt{ d }) \frac{1}{y} \\
& \hspace{98pt}= \frac{1}{y}+2\sqrt{ d } \leq 1+2\sqrt{ d }.
\end{align*}
$$

Infinitely many $(x,y)$ in $\mathbb{Z}^+$ such that $|x-y\sqrt{ d }| < \frac{1}{y}$ $\rightarrow$ $x^2-dy^2=$ integer with absolute value $\leq 2\sqrt{ d }+1$, which means there are finitely many possibilities.

Pigeonhole principle $\implies$ there's $M\in \mathbb{Z}$ with $|M| \leq 2\sqrt{ d }+1$ that is $x^2-dy^2$ with $|x-y\sqrt{ d }| < \frac{1}{y}$ infinitely often.

For all these $x,y\in \mathbb{Z}^+$ where $x^2-dy^2=M$, consider pairs $(x \bmod |M|, y \bmod |M|)$, which gives $|M|^2$ such options.

Since we have infinitely many $x,y \in \mathbb{Z}^+$ with $x^2-dy^2=M$, by pigeonhole principle among these some $\bmod |M|$ reduction $(x \bmod |M|, y \bmod |M|)$ occurs *more than once*:
	There are pairwise-distinct $x_{1},y_{1},x_{2},y_{2}$ in $\mathbb{Z}^+$ such that $x_{1}^2-dy_{1}^2=M$, $x_{2}^2-dy_{2}^2=M$.
	$x_{1}\equiv x_{2} \bmod |M| \rightarrow x_{1}=x_{2}+Ms$ for some $s\in \mathbb{Z}$.
	$y_{1}\equiv y_{2} \bmod |M| \rightarrow y_{1}=y_{2}+Mt$ for some $t\in \mathbb{Z}$.

$x_{1}+y_{1}\sqrt{ d }=(x_{2}+Ms)+(y_{2}+Mt) \sqrt{ d }$
$x_{1}+y_{1}\sqrt{ d } = x_{2}+y_{2}\sqrt{ d }+M(s+t\sqrt{ d })$
$x_{1}-y_{1}\sqrt{ d }=x_{2}-y_{2}\sqrt{ d }+M(s-t\sqrt{ d })$
$M=x_{2}^2-dy_{2}^2=(x_{2}+y_{2}\sqrt{ d })(x_{2}-y_{2}\sqrt{ d })$

$\rightarrow x_{1}+y_{1}\sqrt{ d }=x_{2}+y_{2}\sqrt{ d }+9x_{2}+y_{2}\sqrt{ d })(x_{2}-y_{2}\sqrt{ d })(s+t\sqrt{ d })$
$=(x_{2}+y_{2}\sqrt{ d })(1+(x_{2}-y_{2}\sqrt{ d })(s+t\sqrt{ d }))=x+y\sqrt{ d }$ for some $x,y\sqrt{ d }$

$x_{1}+y_{1}\sqrt{ d }=(xw+y_{2}\sqrt{ d })(x+y\sqrt{ d })$

Apply norms:
$N(x_{1}+y_{1}\sqrt{ d })=N(x_{2}+y_{2}\sqrt{ d })N(x+y\sqrt{ d })$
$x_{1}^2-dy_{1}^2=(x_{2}^2-dy_{2}^2)(x^2-dy^2)$
$M=M(x^2-dy^2) \implies x^2-dy^2=1$

Could $y$ be $0$? Then $x=\pm 1$, so $x_{1}+y_{1}\sqrt{ d }=(x_{2}+y_{2}\sqrt{ d })(\pm 1) = \pm (x_{2}+y_{2}\sqrt{ d })$
$x_{1},x_{2},y_{1},y_{2}$ in $\mathbb{Z}^+ \implies x_{1}=\pm x_{2}, y_{1}=\pm y_{2}$ (same sign)
$\implies x_{1}\not = -x_{2},y_{1}\not = -y_{2}$.
Thus $x_{1}=x_{2}$ and $y_{1}=y_{2}$, which violates how we picked $x_{1},x_{2},y_{1},y_{2}$.