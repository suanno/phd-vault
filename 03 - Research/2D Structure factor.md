#structurefactor #2D #randinit #liquids 

Like in the 1D case ([[1D Structure factor]]) I define:

**I define** the (2D) structure factor

$$S(q_x,q_y)\equiv <|\int e^{-i\mathbf{q}\cdot\mathbf{x}}u(\mathbf{x}) dxdy|^2>$$
where:
- $|...|^2=(...)^*(...)$ is the norm.
- $<...>$ is an average over multiple simulations, all starting from a **random initial condition** (different each time).

### There is a problem - Need a function of ONE variable!
In 2D the structure factor is a function of two variables: $q_x, q_y$. While in all the articles it is presented a function of only one variable! So how do we compute this quantity $\hat{S}(q)$ from $S(q_x, q_y)$?

#### My idea
As there are **no preferential directions**, I expect that the structure factor is a function only of $q=|\mathbf{q}|$ and not of the direction. As a consequence, it is possible to choose a direction in q-space (passing through the origin) and evaluate $S(\mathbf{q})$ along that direction.
So the most simple way of extimating $\hat{S}(q)$ is to evaluate $S(q_x,q_y)$ along the direction $q_x=0$ and along $q_y=0$ and then take the average.
$$\hat{S}(q) = \frac12[S(q,0)+S(0,q)]$$
(considering other directions is not an available option, as in the other directions the points of the lattice are separated by a different distance, so we cannot compare the functions associated to those lines with the horizontal and vertical lines).
This approach of evaluating $S(\mathbf{q})$ along one direction is **motivated** by what happens experimentally with 3D liquids, ==where **to sample one point of the spectrum** $\hat{S}(q)$ the structure factor is **sampled at only one vector** $\mathbf{q}$ with that norm.== So they do not measure multiple vectors to take then an average, as they fix the angle $\varphi$ of the detector's position.
See [[Structure factor in liquids]] for a **motivation** of the present approach.

Here $C = 0.5$ **constant**.

| ![[num_real=10.png]] | ![[num_real=5.png]] |
| -------------------- | ------------------- |

 ![[]]


| ![[t=1_dt=0.01.png]] | ![[20.png]]    |
| -------------------- | -------------- |
| ![[50.png]]          | ![[t=500.png]] |




