# Chapter 3

### 3.1 Optimization methods

...

### 3.2 Greedy Methods

##### Orthogonal matching pursuit (OMP)

> The first algorithm, called *orthogonal matching pursuit*, adds one index to a target support S^n^ at each iteration and updates a target vector x^n^ as the vector supported on the target support S^n^ that best fits the measurements. 

$$
S^{n+1} = S^n ∪ {jn+1},
\\
jn+1 := argmax􏰊_{􏰋j \in [N]}\{|(A∗(y − Ax^n))j|\}
\tag{OMP1}
$$

$$
x^{n+1} = argmin _{z \in C^N}
\{\parallel y − Az \parallel _2, supp(z) ⊂ S^{n+1}\}
\tag{OMP2}
$$

