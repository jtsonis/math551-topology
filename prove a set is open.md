# Concepts & Proofs

**Recall:** a topological space $(X,$**T**$)$ is a set $X$ equipped with a topology **T**. A topology **T** is a collection of subsets of $X$ that includes &#8709;, $X$, arbitrary unions of subcollections of **T**, and finite intersections of subcollections of **T**. A set $U$ is open only if $U \in $**T**.

**Recall:** a basis **B**---which is a collection of subsets of $X$ such that $\forall x\in X, \exists B\in$**B** such that $x\in B$, and $\forall B_1 \cap B_2 \ni x, \exists B_3\in$**B** such that $x\in B_3 \subseteq B_1 \cap B_2$---generates a topology **T** if for all open sets $U \in$**T**$,\exists B\in$**B** such that $x\in B \subseteq U$.

These definitions feel very abstract at the beginning, but they will feel very familiar with enough practice.

<img src="Images/circle%20photo.png" alt="circle" width="200"/>

In the above image, we let the red space be a set in &#8477;	
&#178; and we let circles be the basis which generates the topology on the plane. We know that a set is open if for any point, we can fit a basis element around the point and remain in the set. Contrast this with a *boundary point*, where a basis element will always stick out of the open set.

As one more note, the $x\in B\subseteq U$ condition for openness really should be considered an "if and only if" condition. Consider $(0,1)$ in the real numbers. Is $(0,1)$ open? In the $$\text{\color{blue}indiscrete topology}$$ **T** = &#123;&#8709;, &#8477;&#125;, the answer is clearly no. However in the standard topology on &#8477;, where **B** = &#123; $(a,b)\mid a,b\in$ &#8477;, $a<b$ &#125;, the set $(0,1)$ is open. Lastly, in the $$\text{\color{red}discrete topology}$$, which contains all subsets of &#8477;, $(0,1)$ is trivially open. All of this is to say that the same set can be open or not depending on the topology, and topologies can be classified by which basis generates them. Therefore we define a set $U$ as being open in $X$ with the condition $x\in B\subseteq U$ for a basis element *from the basis that generates the topology on $X$.*

⍟ (Lemma 1): a set $U$ is open if and only if $\forall x\in U, \exists V$ open such that $x\in V\subseteq U$. ⍟

$\Rightarrow$ If $U$ is open, then $\forall x\in U$, $\exists B\in$**B** such that $x\in B\subseteq U$. Because $x \in B$ implies $x\in B\subseteq B$, these basis elements $B$ are open, satisfying the forward direction with $V:=B$. &#x2611;

$\Leftarrow$ Let **V**$=\bigcup_{i\in\lambda} V_i$ be a union of open sets such that $\forall x\in U$, $\exists V_i \in$**V** such that $x\in V_i \subseteq U$; **V** may include infinitely many sets or as few as one set, but the guarantee is that **V** covers $U$. It is obvious that **V**$\subseteq U$ because each individual $V_i\subseteq U$. Additionally, $U\subseteq$**V** because every point $x\in U$ has with it an open set $V_i\in$**V** such that $x\in V_i\subseteq U$. Therefore **V**$\subseteq U$ &#38; $U\subseteq$**V** implies $U=$**V**, and because arbitrary unions of open sets are open, **V**$=U$ is open. &#x2611;

Sadly, all of this is still very abstract. _Are basis elements not easier to use?_ For some problems, basis elements make computation a piece of cake. For other problems, primarily about topologically continuous functions $f\colon X\colon\rightarrow Y$, using a generalized notion of open sets is more helpful. For example, one popular proof is to show that $X$ is a Hausdorff space if and only if $X-\Delta$ is open, where $\Delta = \{(x,x)\mid x\in X\}$. There is no specific basis for $X$ in this problem, and it does not need one.

⍟ Definition ⍟

First of all, if a set is defined to be in the topology, then it is open. If a set is the arbitrary union of other open sets or is the finite intersection of open sets, then it is open. Consider the finite complement topology, and the set **X**$-\{p\}$ for some $p\in X$ is open since its complement is finite. If a function $f\colon X\rightarrow Y$ is topologically continuous, and $V$ is open in $Y$, then $f^{-1}(V)$ is open in $X$ by definition. The Hausdorff condition guarantees for two distinct points $x\ne y$ in a Hausdorff space that there exist neighborhoods $U,V$ such that $x\in U$, $y\in V$, $U\cap V=$&#8709;; these neighborhoods $U$ and $V$ are open by definition of the Hausdorff condition.

And that is it! Either a set is open by basic definition, or there is an open subset around every point in said set. Technically, these notions are the same, but different strategies serve different problems better.

⍟ Finer Topologies ⍟

A topology $T_1$ is finer than another topology $T_A$ if every open set in $T_A$ is an open set in $T_1$, i.e. $T_1 \supseteq T_A$. Of course, if $U$ is open in $T_A$, then $U$ is open in $T_1$. The reason why this is at the end of the section is because you will almost never solve a problem this directly; rather, you would determine whether one topology is finer than another based on the above strategies.

# Example Questions

1. Recall that &#123; $[a,b)\mid a,b \in$ &#8477;&#125; be the basis that generates the lower limit topology on &#8477; and let &#123; $(a,b)\mid a,b \in$ &#8477;&#125; be the basis that generates the standard topology on &#8477;. Prove that $(0,1)$ is open in the lower limit topology. Prove that $[0,1)$ is not open in the standard topology.
* All open sets in a topology can be written as the arbitrary union of and/or the finite intersection of other open sets, but that does not always make it the best strategy. For instance, $(0,1)=\bigcup_{i=2}^\infty [1/n,1)$ which is open in the lower limit topology, but *there is an easier proof* to show that $[0,1)$ is open in the lower limit topology by using (Lemma 1).
* To show that $[0,1)$ is not open in the standard topology, focus on $x = 0$ which might affect the $\forall x\in [0,1)$ criterion from (Lemma 1).

2. Prove that &#8474; is not open. Prove that &#8477; $-$ &#8474; is not open either.

3. If $X = [0,1) \cup \{2\}$, is $[0,1)$ open in the order topology? Is $[0,1]$? Is $\{2\}$ open?
* Recall that the basis for the order topology is all sets $(a,b)$, as well as $[\text{MIN}, a)$ and $(a, \text{MAX}]$.

4. Let $U$ be an open set and let $D$ be a set that is not open. Can $U \cup D$ be open? Can $U \cap D$ be open?
* Use set theory.

5. Show that if $U$ is open in $X$ and $X - A$ is open in $X$, then $U - A$ is open and $X - (A - U)$ is open.
* Use set theory.

6. Let &#8477; have the standard topology. Write an example of an open set in &#8477; × &#8477; using the product topology. Can you draw it?
* Recall that the basis for the product topology of $A \times B$ is &#123; $U \times V \mid U \text{ is open in }A, V \text{ is open in }B$ &#125;.
