# Chapter 1

*An Invitation to Compressive Sensing*

- *标准压缩感知问题*
- *全书内容概括*
- *可能的应用*

### 1.1 什么是压缩感知

$$
Ax=y\tag{1.1}
$$



##### **Sparsity.**



> - How should one design the linear measurement process? In other words, what **matrices A** ∈ C^m×N^ are suitable?
> - How can one reconstruct x from y = Ax? In other words, what are efficient **reconstruction algorithms**?



##### **Algorithms.** 

$l_0$ - minimization 

$\parallel x \parallel _0$ : the number of nonzero entries of a vector x


$$
minimize \parallel z \parallel _0 subject \ to \  Az = y.
$$

$$
\Downarrow
$$

$$
minimize \parallel z \parallel _1 subject \ to  \ Az = y.				

\tag{1.2}
$$



##### **RandomMatrices.** 

> Simple examples are **Gaussian matrices** whose entries consist of independent random variables following a standard normal distribution and **Bernoulli matrices** whose entries are independent random variables taking the values +1 and −1 with equal probability.

##### bound:

$$
m \geq Csln(N/s)

\tag{1.3}
$$

> an m × N Gaussian or Bernoulli matrix A*
>
> all s-sparse vectors x 
>
>  C > 0 is a universal constant (independent of s, m, and N )



##### **Stability.**

quadratically constrained $l_1$-minimization
$$
minimize \parallel z \parallel _1 subject \ to  \ \parallel Az = y\parallel _2 \leq η.			

\tag{1.4}
$$


### 1.2 应用、动机和扩展

##### 单像素相机

##### 磁共振成像

##### 雷达

##### 抽样理论

##### 稀疏近似

##### 纠错

##### 统计与机器学习

#### ==低秩矩阵恢复和矩阵完成==

**Low-Rank Matrix Recovery and Matrix Completion**

 $x ∈ C^N  \ \Rightarrow \  X ∈ C^{n_1×n_2}$

$ Sparsity  \ \Rightarrow \ low \ rank$
$$
minimize \ rank(Z) \ subject \ to \ A(Z) = y
$$

##### the singular value decomposition of X

$$
X=\sum^{n}_{l=1}{σ_lu_lv_l^*}
$$

> $n = min \{n_1,n_2\}$, σ~1~ ≥ σ~2~ ≥ ···σ~n~ ≥ 0 are the singular values of X, and $u_l ∈ C^{n_1}$ , $v_l ∈ C^{n_2}$ are the left and right singular vectors

$rank(X)=\parallel σ(X) \parallel _0$

##### *nuclear norm*

( the $l_1$-norm of the singular value)

$\parallel X \parallel _* =\parallel σ(X) \parallel _1 = \sum^{n}_{l=1}{σ_l(X)}$

##### the nuclear norm minimization problem:

$$
minimize \ \parallel Z \parallel _* \ subject \ to \ A(Z) = y
\tag{1.10}
$$

##### bound:

$$
m \geq Cs \ max\{n_1,n_2\} 
$$

### 1.3 概括全书



