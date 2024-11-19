#structurefactor #1D #randinit #twokinks

### For random initial conditions
I **define** a quantity called **the (1D) structure factor**

$$S(q)\equiv <|\int e^{-iqx}u(x) dx|^2>=<|u_q|^2>$$
where:
- $|...|^2=(...)^*(...)$ is the norm.
- $<...>$ is an average over multiple simulations, all starting from a **random initial condition** (different each time).
### For two isolated kinks
Above we stated the definition of the structure factor, that requires to calculate an average over an ensemble of initial states. Although it could be interesting to consider this quantity also when studying the dynamics of two isolated kinks, so where the initial state is well defined (there is no concept of "ensemble of initial states"). In this case, we just define it without taking the average:
	$$S(q)\equiv |u_q|^2 = u_q u_{-q}$$
where $u_q \equiv e^{-iqx} u(x) dx$

Within the simulations, we compute the Fourier transform using FFTW, so there is no normalization factor in front of the integral.

# Random initial conditions
![[time.png]]
I **cannot see two peaks** related to the domain size and interface's thikness wavelenghts.

I can only see a change in the slope. And the value $q$ at which this happens gets closer to $q=0$ as time passes. I think it represents the large wavelenght (domain size).

Instead, the short wavelenght (interface thikness) should be located at
$$\lambda \sim \sqrt{2/\bar{C}}=2$$
$$q=2\pi/\lambda \sim \pi$$

but I cannot see anything at $q\sim \pi$.
**But** if I plot $q^2 S(q)$, that is the quantity to look for calculating $\braket{q^2}$
![[q2Sq.png]]
# Two isolated kinks
Here the initial state is prepared by composing two stationary state with $C=0.5$, at an initial distance $d_0 = 20,200,400,800$, while $L=1024$, $dx=0.1$.
So the value of u(x) within the domains and the shape and width of the interfaces are "already correct" from the beginning, as the adopted value of C is $C=0.5$.
We do not see any change in the structure factor, because the evolution is very slow.
- $d_0 = 20$

| ![[98 - Images/twokinks/l0=20/state.png]] | ![[98 - Images/twokinks/l0=20/Sq.png]] | ![[98 - Images/twokinks/l0=20/Sqzoom.png]] |
| ----------------------------------------- | -------------------------------------- | ------------------------------------------ |





- $d_0 = 200$ 

| ![[98 - Images/twokinks/l0=200/state.png]] | ![[98 - Images/twokinks/l0=200/sq.png]] | ![[98 - Images/twokinks/l0=200/sqzoom.png]] |
| ------------------------------------------ | --------------------------------------- | ------------------------------------------- |
|                                            |                                         |                                             |


- $d_0 = 400$

| ![[98 - Images/twokinks/l0=400/sq.png]] | ![[98 - Images/twokinks/l0=400/sqzoom.png]] |
| --------------------------------------- | ------------------------------------------- |
|                                         |                                             |



- $d_0 = 800$

| ![[98 - Images/twokinks/l0=800/sq.png]] | ![[98 - Images/twokinks/l0=800/sqzoom.png]] |
| --------------------------------------- | ------------------------------------------- |
|                                         |                                             |




**Notice**: When $l > L/2$ (e.g. when $l=800$) the spectrum becomes less intense. The idea is that, in this case, the complementary domain (we are using PBC) is smaller than $L/2$.

# Periodic states
The following states were prepared in this way
- The state is prepared as $u(x)=\sin(2\pi x/\lambda)$ where $\lambda=L/n$ and n is the number of periods;
- Then that state is evolved with TDGL with $C=1$ constant for a long time to see kinks.

| ![[1period.png]]  | ![[2period.png]]   |
| ----------------- | ------------------ |
| ![[5periods.png]] | ![[10periods.png]] |
