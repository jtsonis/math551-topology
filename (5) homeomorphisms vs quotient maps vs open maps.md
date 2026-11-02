# Homeomorphisms vs Quotient Maps vs Open Maps

**Recall:** a function $f:X\rightarrow Y$ is continuous when $U$ open in $Y$ implies $f^{-1}(U)$ is open in $X$.

Let $f:X\rightarrow Y$ be a function. $f$ is an _open map_ if for all $U$ open in $X$, $f(U)$ is open in $Y$. $f$ is a _quotient map_ if $V$ is open in $Y$ if and only if $f^{-1}(V)$ is open in $X$. $f$ is a homeomorphism if both $f$ and $f^{-1}$ are continuous. Finally, a subset $C$ of $X$ is _saturated_ if it equals the complete inverse of a set in $Y$, i.e. $\exists D$ such that $f^{-1}(D)=C$.
> An alternative definition of quotient maps is that they send saturated open sets in $X$ to open sets in $Y$.

## All Homeomorphisms are Quotient Maps.

Let $f:X\rightarrow Y$ be a homeomorphism. Because $f$ and $f^{-1}$ exist, $f$ is a surjective map (because $f$ is bijective). Let $V$ be an open set in $Y$, and clearly $f^{-1}(V)$ is open in $X$ since $f$ as a homeomorphism is continuous. Now let $S$ be a set in $Y$ such that $f^{-1}(S)$ is open in $X$. Because $f$ is bijective, $f=(f^{-1})^{-1}$, therefore $(f^{-1})^{-1}[f^{-1}(S)]=S$ which is open in $Y$ because $f^{-1}$ is continuous. Therefore a set $U$ is open in $Y$ if and only if $f^{-1}(U)$ is open, meaning $f$ is a quotient map. ☑

## Not all Quotient Maps are Open Maps.

Trivially, all open maps are quotient maps because if every open set maps to an open set, then every saturated open set maps to an open set. However consider the following map $p:X\rightarrow Y$ where $X$ and $Y$ are both subspaces of ℝ using the standard topology. Example Questions #2 and #3 ask you to prove that $p$ is a quotient map, however $p$ is not an open map because the image of $[0,1]$ is $[0,1] \cup &#9128; 2 &#9129;$ which is not open.

<img src="Images/quotientmap.png" alt="quotient map" width="300"/>




## 

## Format ⍟ ☑

# Example Questions
1. Prove that all homeomorphisms are open maps without invoking quotient maps.
2a. Consult the above diagram. Prove that for all basis elements $(a,b)$ in $[0,1]$, $p^{-1}[(a,b)]$ is open.
2b. 
3. Let $f:ℝ\rightarrow ℝ$ via $f(x) = x^2$. Is $[-2,2]$ a saturated set in $X$? Is $[0,2]$ a saturated set in $X$?
4. Closed maps send all closed sets to closed images. Prove that $f:ℝ\rightarrow ℝ$ via $x\mapsto 2$ is a closed. Is $f$ open?
