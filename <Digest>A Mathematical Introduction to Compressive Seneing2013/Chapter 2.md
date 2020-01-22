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
> minimize \parallel z \parallel _0 \ subject \ to \ Az = y. \tag{P0}
> $$
>

(a)(b)