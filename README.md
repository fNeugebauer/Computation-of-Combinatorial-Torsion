# Computation-of-Combinatorial-Torsion
We implemented, among others, the following functions in SageMath:
1. A function with has input a  simplicial set $X$ and a normal subgroup $N\subseteq \pi_1(X)$ with finite index. The function returns a covering projection $p: Z\to X$ such that $p_*\pi_1(Z) = N$ and $Z$ is connected. 
2. A function with has input a  simplicial set $X$ and a normal subgroup $N\subseteq \pi_1(X)$ with finite index. The function returns a covering projection $p: Z\to X$ such that $p_*\pi_1(Z) = N$, $Z$ is connected and $p$ is given as the pullback of a universal covering projection  $\sk_{\dim(X)}(EG) \to  \sk_{\dim(X)}(BG)$, where $G:=\pi_1(X)/N$. 
3. A function that constructs the join of two simplicial sets, as well as, a function that constructs the join of morphisms of simplicial sets.
4. A function that constructs the lens space $L(p;q_1,\dots, q_n)$ for given $p\in \mathbb{N}_{>0}$ and $q_1,\dots, q_n\in \mathbb{Z}$. 
5. A function that computes the combinatorial torsion of a bounded, based chain complex of finite-dimensional $\mathbb{C}$-vector spaces. 
6. A function that computes the Reidemeister torsion of a given simplicial set $X$ for a given finite-dimensional complex representation $\phi: \pi_1(X)\to \mathbb{C}^n$ of the fundamental group of $X$.
7. A function that has input a simplicial set $X$ with finite fundamental group $G$ and returns the Reidemeister torsions of $X$ with respect to all complex irreducible representations of $G$. 

Moreover, we computed, among others, the following examples: 
1. Some finite index covering spaces of the torus and the surface of genus $2$. 
2. The Reidemeister torsions of the following lens spaces:
		$$L(5;1,1), \;L(4;1,3,1),\; L(5;2,3),\; L(7;1,1),\; L(7;1,2),\; \mathbb{R}P^3.$$
		We compared these numbers to the theoretical results in \cite[thm. 10.6]{turaev}.
3. The Reidemeister torsions of the Poincar\'e homology sphere. 
4. The Reidemeister torsions of the following products:
		$$S_2 \times \mathbb{R}P^3,\; L(3;1,1)\times \mathbb{R}P^2,\; L(3;1,1)\times S^2,\; L(3;1,2)\times \mathbb{R}P^2,$$
    $$ L(3;1,2)\times S^2, \;L(3;1,2)\times L(3;1,1),\; L(3;1,2)\times \mathbb{C}P^2,\; \mathbb{R}P^3\times \mathbb{C}P^2.$$
		These examples all satisfied the formula $\tau(X\times Y , \phi\otimes \psi)=\tau(X,\phi)^{\chi(Y)} \tau(Y, \psi)^{\chi(X)}$ for $\phi,\psi$ representations of $\pi_1(X)$ and $\pi_1(X)$, respectively.
