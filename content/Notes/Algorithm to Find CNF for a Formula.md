#definition #logic 

#### Definition
In order to find a CNF for a formula $\varphi$,
##### Step 1
Make a truth table for $\varphi$.

##### Step 2
For each row in which $\varphi$ gets value $0$, form a disjunction consisting of each variable in row with value $0$ and the negation of each variable with value $1$.

Note that if there are no rows with $\varphi$ getting value $0$, so $\varphi$ is a tautology, then we can take $p \vee \neg p$.

##### Step 3
Take conjunction of these disjunctions.

#### Examples


