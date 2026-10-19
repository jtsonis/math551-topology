**Recall:** a topological space $(X,$**T**$)$ is a set $X$ equipped with a topology $\mathcal{T}$. A topology **T** is a collection of subsets of $X$ that includes $\varnothing$, $X$, arbitrary unions of subcollections of **T**, and finite intersections of subcollections of **T**. A set $U$ is open only if $U \in \mathcal{T}$.

**Recall:** a basis **B**---which is a collection of subsets of $X$ such that $\forall x\in X, \exists B\in$**B** such that $x\in B$, and $\forall B_1 \cap B_2 \ni x, \exists B_3\in$**B** such that $x\in B_3 \subseteq B_1 \cap B_2$---generates a topology **T** if for all open sets $U \in$**T**$,\exists B\in$**B** such that $x\in B \subseteq U$.

These definitions feel very abstract, but I hope that they will feel very familiar with enough practice.

<img src="Images/circle%20photo.png" alt="circle" width="200"/>

In the above image, we let the red space be a set in **R**$^2$ and we let circles be the basis which generates the topology on the plane. We know that a set is open if for any point, we can fit a basis element around the point and remain in the set. Contrast this with a *boundary point*, where a basis element will always stick out of the open set.

(Lemma 1): a set $U$ is open if and only if $\forall x\in U, \exists B\in$**B** such that $x\in B\subseteq U$.

(Lemma 2): a set $U$ is open if and only if $\forall x\in U, \exists V$ open such that $x\in V\subseteq U$.

The $\Leftarrow$ proof of (L1) is trivial because that is the definition of **B** generating topologies. Now assume by contradiction that there exists a set $U$ which is open but $\exists x\in U$ where no $B\in$**B** satisfies $x\in B\subseteq U$.

$\Leftarrow$ Recall that $U$ being open means that for said $x\in U, \exists B\in$**B** such that $x\in B\subseteq U$, and because $B$ is open, $V:=B$ satisfies $x\in V\subseteq U$, proving the backward direction. &#x2611;
