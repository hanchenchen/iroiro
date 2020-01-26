# Chapter 2

### 2.1 Sparsity and Compressibility

##### Definition 2.1. 

$x \in C^N$  

$supp(x):=\{j \in [N]:x_j\neq 0 \} . $

$s-sparse$——$\parallel x\parallel _0 := card(supp(x)) \leq s .$

$the \ l_0-norm \ of\  x$ （0-范数）
$$
1_{\{x_j\neq0\}=}
\begin{cases} 
1, \ x_j\neq 0\\ 
0, \ x_j =  0\\
\end{cases} 
$$

##### Definition 2.2. 

$p>0$,$x∈C^N$, the $l_p$*-error of best* s*-term approximation:*
$$
σ_s(x)_p :=inf \{ \parallel x−z\parallel _p, z∈C^N is\ s-sparse \}.
$$
the *unit* $l_p$-*ball:*
$$
B_p^N :=\{z∈C^N :\parallel z \parallel p \leq 1\}.
$$
##### Definition 2.3. 

$any\ q>p>0$,$any\ x∈C^N$:
$$
σ_s(x)_p \leq
\displaystyle \frac{1}{s^{1/p-1/q}}
\parallel x\parallel_p
$$

##### Definition 2.4. 

the *nonincreasing rearrangement* of the vector x

 x^∗^ ∈ R^N^:
$$
x^∗_1 \geq x^∗_2 \geq...\geq x^∗_N \geq 0
$$
证明2.3.

##### **Theorem 2.5.**

$any\ q>p>0$,$any\ x∈C^N$:
$$
σ_s(x)_p \leq
\displaystyle \frac{c_{p,q}}{s^{1/p-1/q}}
\parallel x\parallel_p
$$
*holds with*
$$
c_{p,q}:=[( \frac{p}{q})^{p/q}(1-\frac{p}{q})^{1-p/q}]^{1/p} \leq 1
$$


##### ...



### 2.2 Minimal Number of Measurements

> The compressive sensing problem consists in reconstructing an s-sparse vector x ∈ CN from
>
> $y = Ax$
>
> where $A \ \in C^{m×N}$ is the so-called measurement matrix. With m < N , this system of linear equations is underdetermined, but the sparsity assumption hopefully helps in identifying the original vector x.



$matrix \  A ∈ C^{m×N} , and \ s-sparse \ x ∈ C^N $

> 
(a) The vector x is the unique s-sparse solution of Az = y with y = Ax, that is, $\{z \in C^N :Az=Ax,\parallel z\parallel _0 \leq s\}=\{x\}.$

> (b)The vector x can be reconstructed as the unique solution of
> $$
> minimize \parallel z \parallel _0 \ subject \ to \ Az = y. \tag{P0}\label{eq:P0}
> $$
>

$(a) \Leftrightarrow (b)$



#### Recovery of All Sparse Vectors

$A_S$ ：A的第S个列向量

$x_S$：x的第S个元素



##### Theorem2.13.

*Given* $A\in C^{m×N}$*,the following properties are equivalent :*

> (a)  Every $s-sparse \ vector \ x \in  C^N$ is the unique *s-sparse* solution of $Az = Ax$, that is, if *Ax = Az* and both *x* and *z* are *s-sparse*, then *x = z*. 
>
> (b)  The null space *ker A* does not contain any *2s-sparse*  vector other than the zero vector, that is, *ker A* ∩ $\{z \in C^N :\parallel z\parallel _0 \leq 2s\}=\{0\}$.
>
> (c)  For every $S \subset [N]$ with $card(S) ≤ 2s$, the $submatrix \ A_S$ is injective as a map from C^S^ to C^m^.
>
> (d)  Every set of *2s* columns of *A* is linearly independent.



##### Theorem2.14.

*For any integer* N ≥ 2s*, there exists a measurement matrix* A ∈ C^m×N^ *with* m = 2s *rows such that every* s*-sparse vector* x ∈ C^N^ *can be recovered from its measurement vector* y = Ax ∈ C~m~ *as a solution of* $\ref{eq:P0}$*.*

##### Theorem2.15.

*For any* N ≥ 2s*, there exists a practical procedure for the reconstruction of every* 2s*-sparse vector from its first* m = 2s *discrete Fourier measurements.*



#### Recovery of Individual Sparse Vectors

##### Theorem2.16.

*Forany*N≥s+1*,givenan*s*-sparsevector*x∈CN*,thereexists a measurement matrix* A ∈ Cm×N *with* m = s + 1 *rows such that the vector* x *can be reconstructed from its measurement vector* y = Ax ∈ Cm *as a solution of*  $\ref{eq:P0}$*.*



### 2.3 NP-Hardness of $l_0$ Minimization

##### Theorem 2.17.

*For any* η ≥ 0*, the* $l_0$*-minimization problem* (P~0,η~) *for general* A∈C^m×N^ *and* y∈C^m^ *is NP-hard.*