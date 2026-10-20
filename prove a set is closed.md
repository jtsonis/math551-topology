# Concepts & Proofs
**Recall:** in a topological space $(X,$**T**$)$, a set $C$ is closed when $X-C$ is open. Additionally, $U$ is open when $X-U$ is closed.

**Recall:** some sets are neither open nor closed, an example being &#8474; in the standard topology on &#8477;.
* **Just because $S$ is not open does not mean $S$ is closed! Just because $S$ is not closed does not mean $S$ is open!**

The meaning of a closed set is directly defined by the meaning of an open set, so it is very important to know how to prove that sets are open first. Very often, this is sufficient for proving that a set is closed.

⍟ Complements ⍟

Consider $[0,1]$ in the standard topology on the real line. The complement of $[0,1]$ is $(-\infty,0)\cup(1,\infty)$, and this set is open: for $p\in(-\infty,0)\cup(1,\infty)$, the open interval $(\min\{p,2p\},\max\{p,2p\})$ satisfies $p\in(\min\{p,2p\},\max\{p,2p\})\subseteq(-\infty,0)\cup(0,\infty)$, therefore $(-\infty,0)\cup(1,\infty)$ is open and its complement $[0,1]$ is closed.

⍟ Limit Points ⍟

The formal definition of a limit point $x$ of $A$ is $\forall U$ open with $x\in U$, $(U-\{x\})\cap A\ne \varnothing$, meaning that every open neighborhood around a point intersects the set $A$ at a *distinct point*. This is written as $x\in A'$.

Consider $(0,1)$. Neither $0$ nor $1$ are points in this set, however they are limit points because $0\in(a,b)$ and $(a,b)-\{0\}$ always intersects $(0,1)$ at $(0,\min\{b,1\})$, and $1\in(c,d)$ always intersects at $(\max\{0,a\},1)$. In the below picture, there is an illustration of open sets around $0$ always intersecting the interval $(0,1)$, though it should not be taken literally because open sets in &#8477; look like straight lines, not circles.

<img src="Images/circle-(0,1).png" alt="circle" width="250"/>

(Lemma 2): 

To prove the $\Rightarrow$ direction, assume by way of contradiction that $C$ is closed, $x\in C'$, however $x\not\in C$. As a complement, $x $

⍟ (Lemma 2): a set $C$ is closed if only if it contains all of its limit points, or $C' \subseteq C$. ⍟

$\Rightarrow$ If $U$ is open, then $\forall x\in U$, $\exists B\in$**B** such that $x\in B\subseteq U$. Because $x \in B$ implies $x\in B\subseteq B$, these basis elements $B$ are open, satisfying the forward direction with $V:=B$. &#x2611;

$\Leftarrow$ Let **V**$=\bigcup_{i\in\lambda} V_i$ be a union of open sets such that $\forall x\in U$, $\exists V_i \in$**V** such that $x\in V_i \subseteq U$; **V** may include infinitely many sets or as few as one set, but the guarantee is that **V** covers $U$. It is obvious that **V**$\subseteq U$ because each individual $V_i\subseteq U$. Additionally, $U\subseteq$**V** because every point $x\in U$ has with it an open set $V_i\in$**V** such that $x\in V_i\subseteq U$. Therefore **V**$\subseteq U$ &#38; $U\subseteq$**V** implies $U=$**V**, and because arbitrary unions of open sets are open, **V**$=U$ is open. &#x2611;


&#x2611;
