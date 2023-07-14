# Computation-of-Combinatorial-Torsion
The Reidemeister torsion is a well-known invariant in the field of algebraic topology, but is generally difficult to calculate in practice. We developed an algorithm that calculates the Reidemeister torsion of the geometric realization of a simplicial set. We implemented the algorithm in SageMath and used it to numerically calculate the Reidemeister torsions of the Poincar\'e homology 3-sphere with respect to all irreducible complex representations of its fundamental group. Similar calculations were also performed for several lens and product spaces.  
To obtain the algorithm for Reidemeister torsion we also touched upon the topic of torsions of chain complexes, as well as, on the topic of coverings of simplicial sets. So, also algorithms in the field of those concepts were devoloped. 
We implemented, among others, the following functions in SageMath:
1. A function with has input a  simplicial set $X$ and a normal subgroup $N\subseteq \pi_1(X)$ with finite index. The function returns a covering projection $p: Z\to X$ such that $p_*\pi_1(Z) = N$ and $Z$ is connected. 
2. A function with has input a  simplicial set $X$ and a normal subgroup $N\subseteq \pi_1(X)$ with finite index. The function returns a covering projection $p: Z\to X$ such that $p_*\pi_1(Z) = N$, $Z$ is connected and $p$ is given as the pullback of a universal covering projection  $sk_{\dim(X)}(EG) \to  sk_{\dim(X)}(BG)$, where $G:=\pi_1(X)/N$. The function returns the pullback square. 
3. A function that constructs the join of two simplicial sets, as well as, a function that constructs the join of morphisms of simplicial sets.
4. A function that constructs the lens space $L(p;q_1,\dots, q_n)$ for given $p\in \mathbb{N}_{>0}$ and $q_1,\dots, q_n\in \mathbb{Z}$. 
5. A function that computes the combinatorial torsion of a bounded, based chain complex of finite-dimensional $\mathbb{C}$-vector spaces. 
6. A function that computes the Reidemeister torsion of a given simplicial set $X$ for a given finite-dimensional complex representation $\phi: \pi_1(X)\to \mathbb{C}^n$ of the fundamental group of $X$.
7. A function that has input a simplicial set $X$ with finite fundamental group $G$ and returns the Reidemeister torsions of $X$ with respect to all complex irreducible representations of $G$. 

Moreover, we computed, among others, the following examples: 
1. Some finite index covering spaces of the torus and the surface of genus $2$. 
2. The Reidemeister torsions of the following lens spaces:
		$$L(5;1,1), \quad L(4;1,3,1), \quad  L(5;2,3),  \quad L(7;1,1), \quad  L(7;1,2),  \quad \mathbb{R}P^3.$$
		We compared these numbers to the theoretical result, which for example can be found in Turaev's book "Introduction to Topological Torsion" in theorem 10.6.
3. The Reidemeister torsions of the Poincar\'e homology sphere. 
4. The Reidemeister torsions of the following products:
		$$S_2 \times \mathbb{R}P^3,\quad L(3;1,1)\times \mathbb{R}P^2,\quad  L(3;1,1)\times S^2, \quad L(3;1,2)\times \mathbb{R}P^2,$$
   as well as,
   	$$L(3;1,2)\times S^2, \quad L(3;1,2)\times L(3;1,1), \quad L(3;1,2)\times \mathbb{C}P^2, \quad  \mathbb{R}P^3 \times \mathbb{C}P^2.$$
   These examples all satisfied the formula $\tau(X\times Y , \phi\otimes \psi)=\tau(X,\phi)^{\chi(Y)} \tau(Y, \psi)^{\chi(X)}$ for $\phi,\psi$ representations of $\pi_1(X)$ and $\pi_1(X)$, respectively.
