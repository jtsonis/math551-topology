# Set Theory for Topology

The proofs follow after the results. Remember "iff" is an abbreviation "if and only if." Unless stated otherwise, all sets are subsets of $X$ which is the ambient space.

## Results

* [1] $(A \times C) \cap (B \times D) = (A \cap B) \times (C \cap D)$.
* [2] $A \subseteq B$ iff $X-B \subseteq X-A$.


Let $f\colon X\rightarrow Y$, $A \subseteq X$, $B \subseteq Y$.
* [3] $f(f^{-1}(B)) \subseteq B$; there is equality iff $f$ is injective.
* [4] $A \subseteq f^{-1}(f(A))$; there is equality iff $f$ is surjective.

## Proofs

<img src="Images/product.png" alt="product" width="500"/>

* [1] The above picture should make it visibly clear that $(A \times C) \cap (B \times D) = (A \cap B) \times (C \cap D)$. To prove this rigorously, let $(x,y) \in (A \times C) \cap (B \times D)$, meaning $(x,y) \in A\times C$ and $(x,y) \in B \times D$, thus $x\in A$ and $x\in B$ and $y \in C$ and $y\in D$, therefore $x\in A\cap B$ and $y\in C\cap D$ so $(x,y) \in (A\cap B)\times (C\cap D)$ which proves $(A\times C)\cap(B\times D)\subseteq (A\cap B)\times (C\cap D)$; let $(x,y)\in(A\cap B)\times(C\cap D)$, meaning $x\in A$, $y\in C$, $x\in B$, and $y\in D$ which means $(x,y)\in(A\times C)$ and $(x,y)\in(B\times D)$, therefore $(x,y)\in(A\times C)\cap(B\times D)$ which proves $(A\cap B)\times(C\cap D)\subseteq (A\cap B)\times(C\cap D)$. Therefore these sets are equal.
