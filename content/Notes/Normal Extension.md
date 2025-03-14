#definition #abstract-algebra/field-theory

#### Definition
For ${^{\textstyle E}\big/_{\textstyle k}}$ algebraic (not necessarily finite), we say ${^{\textstyle E}\big/_{\textstyle k}}$ is a *normal extension* if for every $\alpha \in E$, $E$ contains a copy of $\operatorname{split}_{k}m_{{\alpha/k}}(x)$. 

Equivalently, $\alpha \in E$ implies $m_{{\alpha/k}}(x)$ factors $m_{{\alpha/k}}(x) = (x-\alpha_{1})\cdots (x - \alpha_{{\deg(\frac{\alpha}{k})}})$ for some $\alpha_{i} \in E$ that may repeat.

#### Examples
Any $[E:k] \leq 2$ is normal.

If $[E:k] = 1 \implies E=k\ \forall \alpha \in E$, $m_{{\alpha/k}}(x) = x- \alpha$ has "all" roots in $E=k$.
If $[E:k] = 2 \implies \left\{ 1, \alpha \right\}$ is a basis $\forall \alpha \in E \setminus k$.
$\deg m_{{\alpha/k}}(x) = 2$ and $m_{{\alpha/k}}(x) = (x-\alpha)(x- \beta)$ 
($\alpha$ is a root of $m_{{\alpha/k}}(x)$ and $\beta$ is necessarily also in $E$

If $m_{{\alpha/k}}(x) = x^2 + ax + b$ for $a,b \in k$ $\implies$ $\alpha + \beta = -a \implies \beta = -a - \alpha \in E$.

