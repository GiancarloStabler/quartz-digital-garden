#note #analysis/real-analysis 

#### Theorem
The equation $x^{2} =2$ has a unique positive solution in $\mathbb{R}$.

##### Proof
*Existence:* Let $S=\{ x \in \mathbb{R} \mid x \geq 0, x^{2}\leq 2\}$. We want to show that $S$ is bounded above, and that $M=\sup S$ satisfies $M^{2}=2$. If there exists a solution to $x^{2}=2$, then $x=\sup S = \max S = \sqrt{ 2 }$ satisfies $x^2=2$.

$\bar{M}=2$ is an upper bound of $S$. If $x>2 \implies x^{2}>4$ so $x \not\in S$. Thus, by [[the completeness axiom]], $S$ has a supremum. Let $M = \sup S$. We want to show that $M^{2}=2$. Assume for the sake of contradiction that $M^{2} \neq 2$. 

*Case 1:* $M^{2} < 2$.
There exists $\varepsilon > 0$ such that $M^{2} + \varepsilon < 2$. For $\delta > 0$ to be specified below, let $\bar{M} = M + \delta$, so $\bar{M}^{2}=(M + \delta)^{2}=M^{2}+2m\delta+\delta^{2}$. Therefore, $\delta^{2} < \delta$ ($\delta < 1$), and $2M\delta < 4 \delta$ because $M <2$ $\implies \bar{M}^{2} = M^{2} + 2m\delta + \delta^{2} < M^{2} + 5 \delta < (2-\varepsilon)+ 5 \delta$.

For $\delta = \frac{\varepsilon}{5}$ it follows that $\bar{M}^{2}<2 - \varepsilon + 5 \delta = 2$, so $\bar{M} \in S$, which contradicts $M = \sup S$ and $\bar{M} = M + \delta > M$.

*Case 2:* $M^{2} > 2$.
$M^{2} > 2 \implies \exists \varepsilon > 0$ such that $M^{2} > 2 + \varepsilon$. Since $M = \sup S \implies \forall \delta > 0 \exists x = x(\delta) \in S$ so that $x \leq M \leq x + \delta \implies M^{2} \leq (x+\delta)^{2} = x^{2} + 2x\delta + \delta^{2} \leq 2 + 5\delta$. Therefore, $2+\varepsilon < M ^{2} \leq 2 + 5\delta$ contradicts $\delta$ being arbitrary.

Therefore, $M^{2} = 2$.

#### [[Infimum]]

##### Remark
Any set $S$ bounded below has an infimum.

This follows from the completeness axiom.