# Greedy algorithms for compressed sensing

### 8.1 Greed, a flexible alternative to convexification



- ##### "greediness"

- ##### RIP

   A satisfies the *restricted isometry property*



1. ##### Greedy pursuits

   Iteratively \estimation \fast

   theoretical performance guarantees are typically weaker than other methods.

2. ##### Thresholding

   Element selection + pruning

   Fast \easy \guarantees



### 8.2 Greedy pursuits

History 

some notions are all closely related yet discovered independently.

 

#### 8.2.1 General framework

##### 2 fundamental steps:

- Element selection

- coeffient update



##### Initialization:

*estimate:* $\hat x ^{[0]}=0$ 

*initial residual error:* $r^{[0]}=y- \hat x ^{[0]}$

*sipport set(the indices of the nonzero elements):* $T=\emptyset$



##### Algorithm 8.1 General greedy pursuit framework

**Input**: y, A, and k

...



##### Algorithm 8.3 Orthogonal Matching Pursuit(OMP)

**Input:** y, A, and k

**Initialize:** $r^{[0]}=y,\hat x ^{[0]}=0,T=\emptyset$,

**for** $i=1;i:=i+1 \ $till stopping criterion is met **do**

​	$g^{[i]}=A^Tr^{[i-1]}$

​	$$





