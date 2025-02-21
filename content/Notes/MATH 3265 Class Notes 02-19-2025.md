#note #logic/propositional-logic 

### Back to the First Day of the Semester
If it rains ($p$), either Reed remembers his umbrella ($q$) or he gets wet ($r$). It rains ($p$). Reed forgets his umbrella ($\neg q$). Therefore we can infer that he gets wet ($r$).

This gives us that,
$$
\begin{array}{c}
p \rightarrow (q \vee \neg r) \\
p \\
\neg q \\
\hline \\
\therefore r
\end{array}
$$
#### Claim
Any valuation $V$ that satisfies $p \rightarrow (q \vee \neg r)$, $p$, and $\neg q$, must also satisfy $r$.

We can check this with a truth table.

### Defined [[Semantic Consequence]]

#### Fact
Suppose $\Gamma$ is *not* satisfiable. Then $\Gamma \models \varphi$ for every $\varphi$.

This is because $\Gamma \models \varphi$ means that for every valuation in which $\Gamma$ is satisfied, $\varphi$ is also satisfied, which trivially holds when there are no valuations in which $\Gamma$ is satisfied.

#### Fact
Suppose $\Gamma \models \varphi$ and $\Gamma \subseteq \Delta$. Then $\Delta \models \varphi$.

#### Question
Do we always have $\Gamma \models \varphi$ or $\Gamma \models \neg \varphi$.