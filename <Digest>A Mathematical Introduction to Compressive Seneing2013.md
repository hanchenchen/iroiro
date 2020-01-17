# Chapter 1

*An Invitation to Compressive Sensing*

- *标准压缩感知问题*
- *全书内容概括*
- *可能的应用*

### 1.1 什么是压缩感知

$$
Ax=y\tag{1.1}
$$



**稀疏性 Sparsity.**



> - How should one design the linear measurement process? In other words, what **matrices A** ∈ C^m×N^ are suitable?
> - How can one reconstruct x from y = Ax? In other words, what are efficient **reconstruction algorithms**?



*单位矩阵*   the identity matrix

$l_0$ - minimization 

$\parallel x \parallel _0$ : the number of nonzero entries of a vector x
$$
minimize \parallel z \parallel _0 subject \ to \  Az = y.
$$

$$
\Downarrow
$$

$$
minimize \parallel z \parallel _1 subject \ to  \ Az = y.\tag{1.2}
$$

