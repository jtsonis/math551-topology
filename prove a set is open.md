**Recall:** a topological space $(X,$**T**$)$ is a set $X$ equipped with a topology $\mathcal{T}$. A topology **T** is a collection of subsets of $X$ that includes &#8709;, $X$, arbitrary unions of subcollections of **T**, and finite intersections of subcollections of **T**. A set $U$ is open only if $U \in \mathcal{T}$.

**Recall:** a basis **B**---which is a collection of subsets of $X$ such that $\forall x\in X, \exists B\in$**B** such that $x\in B$, and $\forall B_1 \cap B_2 \ni x, \exists B_3\in$**B** such that $x\in B_3 \subseteq B_1 \cap B_2$---generates a topology **T** if for all open sets $U \in$**T**$,\exists B\in$**B** such that $x\in B \subseteq U$.

These definitions feel very abstract, but I hope that they will feel very familiar with enough practice.

<img src="Images/circle%20photo.png" alt="circle" width="200"/>

In the above image, we let the red space be a set in **R**$^2$ and we let circles be the basis which generates the topology on the plane. We know that a set is open if for any point, we can fit a basis element around the point and remain in the set. Contrast this with a *boundary point*, where a basis element will always stick out of the open set.

As one more note, the $x\in B\subseteq U$ condition for openness really should be considered an "if and only if" condition. Consider $(0,1)$ in the real numbers. Is $(0,1)$ open? In the $$\text{\color{blue}indiscrete topology}$$ **T** = {&#8709;, **R**}, the answer is clearly no. However in the standard topology on **R**, where **B** = &#123; $(a,b)\mid a,b\in$ **R**, $a<b$ &#125;, the set $(0,1)$ is open. Lastly, in the $$\text{\color{red}discrete topology}$$, which contains all subsets of **R**, $(0,1)$ is trivially open. All of this is to say that the same set can be open or not depending on the topology, and topologies can be classified by which basis generates them.

(Lemma 1): a set $U$ is open if and only if $\forall x\in U, \exists V$ open such that $x\in V\subseteq U$.

$\Leftarrow$ Recall that $U$ being open means that for said $x\in U, \exists B\in$**B** such that $x\in B\subseteq U$, and because $B$ is open, $V:=B$ satisfies $x\in V\subseteq U$, proving the backward direction. &#x2611;
