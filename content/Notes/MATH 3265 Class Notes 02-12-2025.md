#note #logic 

We want to add a constant $\bot$ to language that denotes $\operatorname{FALSE}$ or $0$. 

#### How to Show a System is NOT Adequate

Suppose we want to show $\left\{ \vee, \wedge \right\}$ is *not* adequate. We must construct a truth table of some formula that has some property that can't be a property of a truth table of any formula created in the system $\left\{ \vee, \wedge \right\}$. For this example, we have that no formula in this system can evaluate to true given that all the variables are have value $0$ (this is a property that needs the $\neg$ operator), and we can prove this inductively.