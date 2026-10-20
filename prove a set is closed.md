# Concepts
**Recall:** in a topological space $(X,$**T**$)$, a set $C$ is closed when $X-C$ is open. Additionally, $U$ is open when $X-U$ is closed.

**Recall:** some sets are neither open nor closed, an example being &#8474; in the standard topology on &#8477;.
> Just because $S$ is not open does not mean $S$ is closed. Just because $S$ is not closed does not mean $S$ is open.

The meaning of a closed set is directly defined by the meaning of an open set, so it is very important to know how to prove that sets are open first. Very often, this is sufficient for proving that a set is closed.

⍟ Complements ⍟

Consider $[0,1]$ in the standard topology on the real line. The complement of $[0,1]$ is $(-\infty,0)\cup(1,\infty)$, and this set is open: for $p\in(-\infty,0)\cup(1,\infty)$, the open interval $(min(p,2p),max(p,2p))$ satisfies $p\in(\min(p,2p),\max(p,2p))\subseteq(-\infty,0)\cup(0,\infty)$, therefore $(-\infty,0)\cup(1,\infty)$ is open
