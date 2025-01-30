#note #logic 

The semantics for a formal language is a way to assign meaning to the expressions in the language.

#### Valuation

*Definition:* a valuation is a function $V: \{ v_{i} \mid i \in \mathbb{N} \} \to \{  0,1 \}$.
- If $V(p)=1$, we say "$V$ makes $p$ true."
- If $V{p}=0$, we say "$V$ makes $p$ false."

*Step 2:* Once we find a valuation $V$, we want to extend it to a function
$$
\hat{V}: \text{ set of all proposition formulae } \to \{  0,1 \}.
$$

We can use recursion to define $\hat{V}$.
$$
\hat{V} = \begin{cases}
V(p) & \text{ if $\alpha$ is a propositional variable $p$}, \\
\dot{\neg}V(\varphi) & \text{ if $\alpha$ is $\neg \varphi$}, \\
\hat{V}(\varphi) \dot{\wedge}\hat{V}(\psi) & \text{ if $\alpha$ is $(\varphi \wedge \psi)$}, \\
\hat{V}(\varphi) \dot{\vee} \hat{V}(\psi) & \text{ if $\alpha$ is $(\varphi \vee \psi)$}, \\
\hat{V} (\varphi) \dot{\rightarrow} \hat{V}(\psi) & \text{ if $\alpha$ is $(\varphi \rightarrow \psi)$}, \\
\hat{V} (\varphi) \dot{\leftrightarrow} \hat{V} (\psi) & \text{ if $\alpha$ is $(\varphi \leftrightarrow \psi)$}.
\end{cases}
$$

I know this is not particularly helpful but it's how we did it in class and I don't want to write the truth tables for the different connectives since I absolutely know them.

#### Defined [[Satisfiable]]

