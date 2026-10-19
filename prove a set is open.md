**Recall:** a topological space $(X, \mathcal{T})$ is a set $X$ equipped with a topology $\mathcal{T}$. A topology $\mathcal{T}$ is a collection of subsets of $X$ that includes $\varnothing$, $X$, arbitrary unions of subcollections of $\mathcal{T}$, and finite intersections of subcollections of $\mathcal{T}$. A set $U$ is open only if $U \in \mathcal{T}$.

**Recall:** a basis $\mathcal{B}$---which is a collection of subsets of $X$ such that $\forall x\in X$, $\exists B\in\mathcal{B}$ such that $x\in B$, and $\forall B_1 \cap B_2 \ni x$, $\exists B_3$ such that $x\in B_3 \subseteq B_1 \cap B_2$---generates a topology $\mathcal{T}$ if for all open sets $U \in \mathcal{T}$, $\exists B\in\mathcal{B}$ such that $x\in B \subseteq U$.

These definitions feel very abstract, but I hope that they will feel very familiar with enough practice.

<img src="Images/circle%20photo.png" alt="circle" width="200"/>

In this image, we let the red space be a set in $\mathbb{R}^2$ and we let circles be the basis which generates the topology on the plane. We know that a set is open if for any point, we can fit a basis element around the point and remain in the set. Contrast this with a *boundary point*, where a basis element will always stick out of the open set.
