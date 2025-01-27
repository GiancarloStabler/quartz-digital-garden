#note #logic 

### [[Propositional Logic]]

#### Notation Convention for this Course
Because it is a pain to write the subscripts on variables, we will tend to use $p,q,r,\ldots$ to denote variables rather than $v_{1},v_{2},v_{3}, \ldots$ .

#### Formation Trees
(Draw trees the same way that we did in PHIL 1102).

##### Example: Recursive Definition
Define a function $F$ on set of all propositional formulas by recursion.

*Base case:* Specify $F(v_{i})$ for each propositional variable $v_{i}$.

*Inductive cases:* 
- Specify $F(\neg \varphi )$ using $F(\varphi)$.
- Specify $F((\varphi \wedge \psi))$ using $F(\varphi)$ and $F(\psi)$.
- Specify $F((\varphi \vee \psi)$ using $F(\varphi)$ and $F(\psi)$.
- Specify $F((\varphi \rightarrow \psi))$ using $F(\varphi)$ and $F(\psi)$.
- Specify $F((\varphi \leftrightarrow \psi))$ using $F(\varphi)$ and $F(\psi)$.

#### Example: Inductive Proof
Prove that every formula has the same number of left and right parentheses.

*Base case:* Show every propositional variable $v_{i}$ has the property $P$.
*Induction cases:* 
- Assume $\varphi$ has property $P$. Show that $\neg \varphi$ also has $P$. 
- Assume $\varphi$ and $\psi$ both have property $P$. Show that $(\varphi * \psi)$ has property $P$ for each of $*= \wedge, \vee, \leftarrow, \leftrightarrow$.

