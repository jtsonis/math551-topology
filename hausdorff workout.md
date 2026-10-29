# Hausdorff Workout

**Recall:** a topological space $X$ is a Hausdorff space if it satisfies the Hausdorff condition, meaning for all distinct $x,y\in X$, $\exists U,V$ open such that $x\in U$, $y\in V$, $U\cap V=\varnothing$.

## ⍟ The Standard Topology on the Reals Is Hausdorff ⍟
Without loss of generality, let $x<y$ be distinct points in ℝ. Their average $z:=(x+y)/2$ satisfies $x<z<y$, thus $x\in(-\infty,z)$, $y\in(z,\infty)$, and $(-\infty,z)\cap (z,\infty)=\varnothing$, satisfying the Hausdorff condition. ☑


# Example Questions
1. The $T_1$ axiom states that all finite point sets are closed. Prove that if $X$ is Hausdorff, then $X$ satisfies the $T_1$ axiom.
* HINT: prove that singletons are closed in Hausdorff spaces, which generalizes to finite point sets since the finite union of closed sets is closed.
