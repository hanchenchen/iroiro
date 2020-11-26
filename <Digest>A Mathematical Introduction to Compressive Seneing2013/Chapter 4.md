# Chapter 4

Basis pursuit 

$l_1 - minimization$



### 4.1 Null Space Property

### ...

### 4.6 Low-Rank Matrix Recovery

##### Theorem 4.40.

*Given a linear map* A *from* $C^{n_1×n_2}$ *to* $C^m$*, every matrix* X ∈ Cn1×n2 *of rank at most* r *is the unique solution of* (4.39) *with* y = A(X) *if and* *only if, for all* M ∈ ker A \ {0} *with singular values* σ~1~(M) ≥ · · · ≥ σ~n~(M) ≥ 0*,* n := min{n~1~, n~2~}*,*
$$
\sum ^{r}_{j=1} σ_j (M) <
\sum ^{n}_{j=r+1} σ_j (M)
\tag{4.40}
$$
