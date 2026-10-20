# Concepts & Proofs
**Recall:** in a topological space $(X,$**T**$)$, a set $C$ is closed when $X-C$ is open. Additionally, $U$ is open when $X-U$ is closed.

**Recall:** some sets are neither open nor closed, an example being &#8474; in the standard topology on &#8477;.
* **Just because $S$ is not open does not mean $S$ is closed! Just because $S$ is not closed does not mean $S$ is open!**

The meaning of a closed set is directly defined by the meaning of an open set, so it is very important to know how to prove that sets are open first. Very often, this is sufficient for proving that a set is closed.

⍟ Complements ⍟

Consider $[0,1]$ in the standard topology on the real line. The complement of $[0,1]$ is $(-\infty,0)\cup(1,\infty)$, and this set is open: for $p\in(-\infty,0)\cup(1,\infty)$, the open interval $(\min\{p,2p\},\max\{p,2p\})$ satisfies $p\in(\min\{p,2p\},\max\{p,2p\})\subseteq(-\infty,0)\cup(0,\infty)$, therefore $(-\infty,0)\cup(1,\infty)$ is open and its complement $[0,1]$ is closed.

⍟ Limit Points ⍟

The formal definition of a limit point $x$ of $A$ is $\forall U$ open with $x\in U$, $(U-\{x\})\cap A\ne \varnothing$, meaning that every open neighborhood around a point intersects the set $A$ at a *distinct point*. This is written as $x\in A'$.

Consider $(0,1)$. Neither $0$ nor $1$ are points in this set, however they are limit points because $0\in(a,b)$ and $(a,b)-\{0\}$ always intersects $(0,1)$ at $(0,\min\{b,1\})$, and $1\in(c,d)$ always intersects at $(\max\{0,a\},1)$. The picture below is an illustration of open sets around $0$ always intersecting the interval $(0,1)$, though it should not be taken literally because open sets in &#8477; look like straight lines, not circles.

<img src="Images/circle-(0,1).png" alt="circle" width="250"/>

⍟ (Lemma 2): a set $C$ is closed in $X$ if only if it contains all of its limit points, or $C' \subseteq C$. ⍟

$\Rightarrow$ If $C$ is closed, then $X-C$ is open by definition. Therefore for every point $p\in X-C$, $\exists U$ open in $X$ such that $p\in U\subseteq X-C$. $U\subseteq X-C$ implies $U\cap C=\varnothing$, therefore $p\not\in C'$ since $U-\{p\}\subseteq U$ which does not intersect $C$. Therefore, none of the points in $X-C$ are in $C'$, thus $C'\subseteq C$. &#x2611;

$\Leftarrow$ Let $C'\subseteq C$. Then $X-C\subsetq X-C'$ by set theory. Thus for any $p\in X-C$, then $p\in X-C'$ which implies $\exists U$ open in $X$ such that $p\in U$ and $U-\{p\}\cap C\subseteq U\cap C=\varnothing$ (for otherwise, $p$ would be a limit point, i.e. $p\in C'$). $U\cap C=\varnothing$ means $U\subseteq X-C$, thus $p\in U\subseteq X-C$. Therefore $X-C$ is open, thus $C$ is closed. &#x2611;

&#x2611;


&#x2611;
