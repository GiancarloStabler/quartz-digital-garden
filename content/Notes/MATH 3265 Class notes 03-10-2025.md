#note #logic/propositional-logic 

#### Summary of Last Week
$\varphi$ is a tautology, $\models \varphi \iff$ for all valuations $V$, $V(\varphi)=1$.
$\varphi$ is provable, $\vdash \varphi \iff$ there is a contradictory finite tableau with root labeled $F\varphi$.

##### Theorem
$\models \varphi \iff \vdash \varphi$. The right direction is the Completeness Theorem, and the left direction is the Soundness Theorem.

##### Extend this Picture
$\Gamma \models \varphi \iff$ for all valuations $V$ such that $V \models \Gamma$, we have $V \models \varphi$ (we say $\varphi$ is a consequence of $\Gamma$).

#### Defined [[Set of Finite Tableau]]

#### Defined [[Tableau Proof]]

Following the defined algorithm generates the **complete systematic tableau from $\Gamma$ with root $F\varphi$**.
- To do this, you need to fix an order on $\Gamma$
- $\Gamma$ could be infinite...we will always assume $\Gamma$ is countable, which just means it can be listed as $\Gamma = \left\{  \gamma_{1},\gamma_{2},\ldots \right\}$ (indices are positive whole numbers).

##### Example
Generate the complete systematic tableau from $\left\{  p_{0} \rightarrow p_{1}, p_{1} \rightarrow p_{2} \right\}$.

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{math}

\begin{tikzcd}[ampersand replacement=\&, row sep = 1em, column sep = 0.5em] \& {F \neg p_0} \\ \& {T p_0} \\ \& {T ( p_0 \rightarrow p_1)} \\ {Fp_0} \&\& {Tp_1} \\ \bot \&\& {T(p_1 \rightarrow p_2)} \\ \& {Fp_1} \&\& {Tp_2} \\ \& \bot \&\& \top \arrow[no head, from=1-2, to=2-2] \arrow[no head, from=2-2, to=3-2] \arrow[no head, from=3-2, to=4-3] \arrow[no head, from=4-1, to=3-2] \arrow[no head, from=4-3, to=5-3] \arrow[no head, from=5-3, to=6-4] \arrow[no head, from=6-2, to=5-3] \end{tikzcd}

\end{math}
\end{document}

```
We can see that there exists a non-contradictory branch (the one ending with $Tp_{2}$) in the complete systematic tableau. 

Define valuation $V$ by $V(p_{0})=1$, $V(p_{1})=1$, and $V(p_{2})=1$. Then check that $V$ agrees with **all** signed formulas on branch.

##### Example
Generate complete systematic tableau from $\Gamma = \left\{  p_{0} \rightarrow p_{1}, p_{1} \rightarrow p_{2}, \ldots \right\}$ with root labeled $F \neg p_{0}$ (trying to check if $\Gamma \vdash \neg p_{0}$).

```tikz 
\usepackage{tikz-cd}

\begin{document}
\begin{math}
\begin{tikzcd}[ampersand replacement=\&, row sep = 1em, column sep = 0.5em] \& {F \neg p_0} \\ \& {Tp_0} \\ \& {T(p_0 \rightarrow p_1)} \\ {F p_0} \&\& {Tp_1} \\ \&\& {T(p_1 \rightarrow p_2)} \\ \& {F p_1} \&\& {Tp_2} \\ \&\&\& {T(p_2 \rightarrow p_3)} \\ \&\&\& \vdots \arrow[no head, from=1-2, to=2-2] \arrow[no head, from=2-2, to=3-2] \arrow[no head, from=3-2, to=4-3] \arrow[no head, from=4-1, to=3-2] \arrow[no head, from=5-3, to=4-3] \arrow[no head, from=5-3, to=6-4] \arrow[no head, from=6-2, to=5-3] \arrow[no head, from=6-4, to=7-4] \end{tikzcd}
\end{math}
\end{document}
```
