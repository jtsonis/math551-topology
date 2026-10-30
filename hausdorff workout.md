# Hausdorff Workout

**Recall:** a topological space $X$ is a Hausdorff space if it satisfies the Hausdorff condition, meaning for all distinct $x,$ $y\in X,$ $\exists U,$ $V$ open such that $x\in U,$ $y\in V,$ $U\cap V=\varnothing$.

## ⍟ (Lemma 4) The Hausdorff Condition Generalizes to $n$ Distinct Elements ⍟
The $n=2$ case follows by definition. Let $n=3,$ and let $a,$ $b,$ $c$ be distinct elements in $X$. By the Hausdorff condition, there exist open sets $U_{ab},$ $V_{ba}$ such that $a\in U_{ab},$ $b\in V_{ba},$ and $U_{ab}\cap V_{ba}=\varnothing,$ and there exist open sets $U_{ac}, V_{ca}$ such that $a\in U_{ac},$ $c\in V_{ca},$ and $U_{ac}\cap V_{ca}=\varnothing,$ and there exist open sets $U_{bc}, V_{cb}$ such that $b\in U_{bc},$ $c\in V_{cb},$ and $U_{bc}\cap V_{cb}=\varnothing$. The intersection of open sets is open, and the sets $A:= U_{ab}\cap U_{ac},$ $B:= V_{ba}\cap U_{bc},$ $C:= V_{ca}\cap V_{cb}$ are open sets such that $a\in A,$ $b\in B,$ and $c\in C$. $A\cap B = (U_{ab}\cap V_{ba})\cap U_{ac}\cap U_{bc}=\varnothing,$ $A\cap C = (U_{ac}\cap V_{ca})\cap U_{ab}\cap V_{cb}=\varnothing,$ and $B\cap C = (U_{bc}\cap V_{cb})\cap V_{ba}\cap V_{ca}=\varnothing$.

Now assume that the Hausdorff condition holds for $k$ distinct elements $x_1,\dots,x_k$ and consider an additional distinct $x_{k+1}$. There exist pairwise disjoint open sets $U_{i}$ such that $x_i \in U_i$ for each $1\le i\le k,$ and there exist open sets $V_i,W_i$ such that $x_i \in V_i,$ $x_{k+1}\in W_i,$ and $V_i\cap W_i=\varnothing$. Let $W := \bigcup W_i$ and $x_{k+1}\in W$ clearly. Additionally $x_i\in U_i\cap V_i$ which are all disjoint from each other since for any $i\ne j,$ $(U_i\cap V_i)\cap(U_j\cap V_j)=(U_i\cap U_j)\cap V_i\cap V_j=\varnothing$. Finally $(U_i\cap V_i)\cap W=U_i\cap(V_i\cap W)=\varnothing$. Therefore if the Hausdorff condition holds for $k$ distinct elements, it holds for $k+1$ distinct elements. By the Principle of Mathematical Induction, the Hausdorff condition generalizes to $n$ distinct elements. ☑

## ⍟ The Standard Topology on the Reals is Hausdorff ⍟
Without loss of generality, let $x<y$ be distinct points in ℝ. Their average $z:=(x+y)/2$ satisfies $x<z<y,$ thus $x\in(-\infty,z),$ $y\in(z,\infty),$ and $(-\infty,z)\cap (z,\infty)=\varnothing,$ satisfying the Hausdorff condition. ☑

## ⍟ The Lower Limit Topology on the Reals is Hausdorff ⍟
Let $x<y$ and $[x,y)\cap [y,\infty)=\varnothing$ satisfies the Hausdorff condition. ☑

## ⍟ The Finite Complement Topology on an Infinite Set is NOT Hausdorff ⍟
Let $x,y\in X$ with $x\ne y$ and assume by contradiction that $\exists U,V$ open such that $x\in U,$ $y\in V,$ and $U\cap V=\varnothing$. By definition, $X-V$ is finite, and $U\cap V=\varnothing$ means $U\subseteq X-V,$ therefore $U$ is finite, thus $U\cup(X-U)=X$ is finite, however $X$ is infinite, thus we have a contradiction. Therefore there cannot exist open sets $U,V$ on distinct points, meaning the Hausdorff condition cannot be met. ☑

## ⍟ The Discrete Topology is Hausdorff ⍟
Let $x$ and $y$ be distinct points in the discrete topology and the singletons $x$ and $y$ are disjoint open sets which contain themselves, satisfying the Hausdorff condition. ☑

## ⍟ The Indiscrete Topology is NOT Hausdorff ⍟
Recall that the indiscrete topology on a set $X$ is &#123; $X,\varnothing$ &#125; so the only open set available to contain two disjoint points is $X,$ and $X\cap X=X\ne\varnothing,$ so the indiscrete topology cannot satisfy the Hausdorff condition. ☑

# Example Questions
1. Prove that all order topologies are Hausdorff.
* HINT: if $x\ne y,$ either $\exists z$ such that $x<z<y$, or $(x,y)=\varnothing.$ These cases have to be examined separately.
2. Prove that the product of two Hausdorff spaces is Hausdorff.
3. Prove that a subspace of a Hausdorff space is Hausdorff.
4. Let $\Delta =$ &#123; $x\times x\mid x\in X$ &#125; be the diagonal of $X$. Prove that $X$ is Hausdorff if and only if $\Delta$ is closed.
* HINT: consider distinct elements $a\ne b$ and $(a,a),(b,b)\in X\times X$.
5. The $T_1$ axiom states that all finite point sets are closed. Prove that if $X$ is Hausdorff, then $X$ satisfies the $T_1$ axiom.
* HINT: prove that singletons are closed in Hausdorff spaces, which generalizes to finite point sets since the finite union of closed sets is closed.
6. Let $X$ be a Hausdorff space with a sequence $x_n$. Prove that if $x_n$ converges to $x$ and $y,$ then $x=y$.
7. Let $f,g: X\rightarrow Y$ be continuous functions and let $Y$ be Hausdorff. Prove that $E:=$ &#123; $x\in X\mid f(x)=g(x)$ &#125; is closed.
* HINT: by definition of topological continuity, for any open sets $U,V\subseteq Y,$ $f^{-1}(U)$ and $g^{-1}(V)$ are open.
* HINT: recall that $E$ is closed if $X-E=$ &#123; $x\in X\mid f(x) \ne g(x)$ &#125; is open, and for all $p\in X-E$, $f(p)$ and $g(p)$ are distinct points in $Y$.
8. Let $A\subseteq X$, let $f:A\rightarrow Y$ be continuous, and let $Y$ be Hausdorff. If it is the case that $g:\bar{A}\rightarrow Y$ and $h:\bar{A}\rightarrow Y$ can be well-defined as continuous extensions of $f$, prove that $g(x) = h(x)$ for all $x\in A$
* HINT: if $x\in A$, then $g(x)=h(x)=f(x)$. The nontrivial points are $x\in\bar{A}-A$.
* HINT: recall that if $x\in \overline{A}$, then $\forall U$ open with $x\in U$, $U\cap A\ne\varnothing$.
