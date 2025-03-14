#definition #logic/proof-theory

#### Definition
A (tableau) proof of $\varphi$ from $\Gamma$ is a contradictory [[finite tableau]] from $\Gamma$ with root labeled $F\varphi$. If $\varphi$ has a (tableau) proof from $\Gamma$, we say $\Gamma$ proves $\varphi$ (or $\varphi$ is provable from $\Gamma$) and write $\Gamma \vdash \varphi$.

#### Examples

Show $\left\{ p \implies (q \vee r) , \neg q, \neg r \right\} \vdash \neg p$.

```tikz
\usepackage{tikz-cd}

\begin{document}
\begin{math}
\begin{tikzcd}[ampersand replacement=\&, row sep = 1em, column sep = 0.5em] \& {F \neg \varphi} \\ \\ \& {T \varphi} \\ \\ \& {T(p\rightarrow(q \vee r))} \\ \\ {F p} \&\& {T(q\vee r)} \\ \bot \\ \& Tq \&\& Tr \\ \\ \& {T\neg q} \&\& {T \neg q} \\ \\ \& Fq \&\& {F q} \\ \& \bot \\ \&\&\& {T\neg r} \\ \\ \&\&\& Fr \\ \&\&\& \bot \arrow[no head, from=1-2, to=3-2] \arrow[no head, from=3-2, to=5-2] \arrow[no head, from=7-1, to=5-2] \arrow[no head, from=7-3, to=5-2] \arrow[no head, from=7-3, to=9-4] \arrow[no head, from=9-2, to=7-3] \arrow[no head, from=9-2, to=11-2] \arrow[no head, from=9-4, to=11-4] \arrow[no head, from=11-2, to=13-2] \arrow[no head, from=11-4, to=13-4] \arrow[no head, from=13-4, to=15-4] \arrow[no head, from=15-4, to=17-4] \end{tikzcd}
\end{math}
\end{document}
```


