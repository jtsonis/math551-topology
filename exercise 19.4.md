# Exercise 19.4

<img src="Images/munkres19.4" alt="19.4 problem" width="500"/>

This one exercise technically contains 21 problems, which can be very overwhelming. Here is an explanation behind every one of them.

### **EVERYTHING BELOW IS ABOUT TUPLES OF REAL NUMBERS!**

## Continuity & Convergence in the Product Topology
Theorem 19.6 states that a function in the product topology is continuous if and only if each coordinate function is continuous. Likewise, Exercise 19.6 proves that a sequence is continuous in the product topology if and only if each coordinate's sequence is continuous. When working with the product topology, go coordinate by coordinate.

These are the answers to each question regarding the product topology:
* $f(t)$ is continuous because each coordinate function $f_n(t)=n\cdot t$ is continuous.
* $g(t)$ is continuous because each coordinate function $g_n(t)=t$ is continuous.
* $h(t)$ is continuous because each coordinate function $h_n(t)=t/n$ is continuous.
* $\vec{w}$ converges to $\vec{0}$ because the *n*'th coordinate of $w_k$ equals $0$ for all $k>n$.
* $\vec{x}$ converges to $\vec{0}$ because the *n*'th coordinate of $x_k$ equals $0$ for all $k>n$.
* Regarding $\vec{y}$, $\forall \varepsilon>0$, there exists a $N\in\mathbb{N}$ such that $N>1/\varepsilon$, leading to the *n*'th coordinate of $|y_k|\le\max\{0,1/k\}<1/N<\varepsilon$ for all $k>N$. Therefore each coordinate converges to $0$ and $\vec{y}$ converges to $\vec{0}$.
* The first and second coordinates of $\vec{z}$ converge to $0$ since $1/n$ converges to $0$, and the other coordinates equal $0$. Therefore $\vec{z}$ converges to $\vec{0}$.

## Continuity in the Box Topology

It is possible for a function to be continuous in the box topology, and that happens when all but finitely many terms are constant (and that should be easy to prove). Every other function is not continuous! Here is the strategy: fix $x \in &#8477;$ and let $B=\displaystyle\prod_{n = 1}^\infty (f_n(x)-1/n,f_n(x)+1/n)$, which is a basis element in the box topology by Theorem 

## Continuity in the Uniform Topology

## Convergence in the Box Topology

## Convergence in the Uniform Topology
