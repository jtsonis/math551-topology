**Recall:** a topological space $(X,$**T**$)$ is a set $X$ equipped with a topology $\mathcal{T}$. A topology **T** is a collection of subsets of $X$ that includes &#8709;, $X$, arbitrary unions of subcollections of **T**, and finite intersections of subcollections of **T**. A set $U$ is open only if $U \in \mathcal{T}$.

**Recall:** a basis **B**---which is a collection of subsets of $X$ such that $\forall x\in X, \exists B\in$**B** such that $x\in B$, and $\forall B_1 \cap B_2 \ni x, \exists B_3\in$**B** such that $x\in B_3 \subseteq B_1 \cap B_2$---generates a topology **T** if for all open sets $U \in$**T**$,\exists B\in$**B** such that $x\in B \subseteq U$.

These definitions feel very abstract at the beginning, but they will feel very familiar with enough practice.

<img src="Images/circle%20photo.png" alt="circle" width="200"/>

In the above image, we let the red space be a set in **R**$^2$ and we let circles be the basis which generates the topology on the plane. We know that a set is open if for any point, we can fit a basis element around the point and remain in the set. Contrast this with a *boundary point*, where a basis element will always stick out of the open set.

As one more note, the $x\in B\subseteq U$ condition for openness really should be considered an "if and only if" condition. Consider $(0,1)$ in the real numbers. Is $(0,1)$ open? In the $$\text{\color{blue}indiscrete topology}$$ **T** = {&#8709;, **R**}, the answer is clearly no. However in the standard topology on **R**, where **B** = &#123; $(a,b)\mid a,b\in$ **R**, $a<b$ &#125;, the set $(0,1)$ is open. Lastly, in the $$\text{\color{red}discrete topology}$$, which contains all subsets of **R**, $(0,1)$ is trivially open. All of this is to say that the same set can be open or not depending on the topology, and topologies can be classified by which basis generates them. Therefore we define a set $U$ as being open in $X$ with the condition $x\in B\subseteq U$ for a basis element *from the basis that generates the topology on $X$.*

⍟ (Lemma 1): a set $U$ is open if and only if $\forall x\in U, \exists V$ open such that $x\in V\subseteq U$. ⍟

$\Rightarrow$ If $U$ is open, then $\forall x\in U$, $\exists B\in$**B** such that $x\in B\subseteq U$. Because $x \in B$ implies $x\in B\subseteq B$, these basis elements $B$ are open, satisfying the forward direction with $V:=B$. &#x2611;

$\Leftarrow$ Let **V**$=\bigcup_{i\in\lambda} V_i$ be a union of open sets such that $\forall x\in U$, $\exists V_i \in$**V** such that $x\in V_i \subseteq U$; **V** may include infinitely many sets or as few as one set, but the guarantee is that **V** covers $U$. It is obvious that **V**$\subseteq U$ because each individual $V_i\subseteq U$. Additionally, $U\subseteq$**V** because every point $x\in U$ has with it an open set $V_i\in$**V** such that $x\in V_i\subseteq U$. Therefore **V**$\subseteq U$ &#38; $U\subseteq$**V** implies $U=$**V**, and because arbitrary unions of open sets are open, **V**$=U$ is open. &#x2611;

Sadly, all of this is still very abstract. _Are basis elements not easier to use?_ For some problems, basis elements make computation a piece of cake. For other problems, primarily about topologically continuous functions $f\colon X\colon\rightarrow Y$, using a generalized notion of open sets is more helpful. For example, one popular proof is to show that $X$ is a Hausdorff space if and only if $X-\Delta$ is open, where $\Delta = \{(x,x)\mid x\in X\}$. There is no specific basis for $X$ in this problem, and it does not need one.

⍟ Definition ⍟

First of all, if a set is defined to be in the topology, then it is open. Consider the finite complement topology, and the set **X**$-\{p\}$ for some $p\in X$ is open since its complement is finite. If a function $f\colon X\rightarrow Y$ is topologically continuous, and $V$ is open in $Y$, then $f^{-1}(V)$ is open in $X$ by definition. The Hausdorff condition guarantees for two distinct points $x\ne y$ in a Hausdorff space that there exist neighborhoods $U,V$ such that $x\in U$, $y\in V$, $U\cap V=$&#8709;; these neighborhoods $U$ and $V$ are open by definition of the Hausdorff condition.
