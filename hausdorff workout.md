# Hausdorff Workout

**Recall:** a topological space $X$ is a Hausdorff space if it satisfies the Hausdorff condition, meaning for all distinct $x,y\in X$, $\exists U,V$ open such that $x\in U$, $y\in V$, $U\cap V=\varnothing$.

## ⍟ The Standard Topology on the Reals is Hausdorff ⍟
Without loss of generality, let $x<y$ be distinct points in ℝ. Their average $z:=(x+y)/2$ satisfies $x<z<y$, thus $x\in(-\infty,z)$, $y\in(z,\infty)$, and $(-\infty,z)\cap (z,\infty)=\varnothing$, satisfying the Hausdorff condition. ☑

## ⍟ The Lower Limit Topology on the Reals is Hausdorff ⍟
Let $x<y$ and $[x,y)\cap [y,\infty)=\varnothing$ satisfies the Hausdorff condition. ☑

## ⍟ The Finite Complement Topology on an Infinite Set is NOT Hausdorff ⍟
Let $x,y\in X$ with $x\ne y$ and assume by contradiction that $\exists U,V$ open such that $x\in U$, $y\in V$, and $U\cap V=\varnothing$. By definition, $X-V$ is finite, and $U\cap V=\varnothing$ means $U\subseteq X-V$, therefore $U$ is finite, thus $U\cup(X-U)=X$ is finite, however $X$ is infinite, thus we have a contradiction. Therefore there cannot exist open sets $U,V$ on distinct points, meaning the Hausdorff condition cannot be met. ☑

## ⍟ The Discrete Topology is Hausdorff ⍟
Let $x$ and $y$ be distinct points in the discrete topology and the singletons $x$ and $y$ are disjoint open sets which contain themselves, satisfying the Hausdorff condition. ☑

## ⍟ The Indiscrete Topology is NOT Hausdorff ⍟
Recall that the indiscrete topology on a set $X$ is &#123; $X,\varnothing$ &#125; so the only open set available to contain two disjoint points is $X$, and $X\cap X=X\ne\varnothing$, so the indiscrete topology cannot satisfy the Hausdorff condition. ☑

# Example Questions
1. The $T_1$ axiom states that all finite point sets are closed. Prove that if $X$ is Hausdorff, then $X$ satisfies the $T_1$ axiom.
* HINT: prove that singletons are closed in Hausdorff spaces, which generalizes to finite point sets since the finite union of closed sets is closed.
