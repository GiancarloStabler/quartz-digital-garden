#definition #logic 

#### Definition
In order to find a DNF for a formula $\varphi$,
##### Step 1
Make a truth table for $\varphi$.

##### Step 2
For each row in which $\varphi$ gets value $1$, form a conjunction consisting of each variable in row with value $1$ and the negation of each variable with value $0$.

Note that if there are no rows with $\varphi$ getting value $1$ ($\varphi$ is a contradiction), then just take $p \wedge \neg p$.

##### Step 3
Take disjunction of these conjunctions.

#### Examples


