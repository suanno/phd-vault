#singlekink #1D #timedependingC
## Question: 
If we have an isolated kink **at the center** of the simulation box
$$u(x,t=0)=\tanh((x-L/2)2^{-\frac{1}2 })$$
(in reality, due to **PBC** we have two kinks, the other is at x=0=L)
and $C=C(t)$ is oscillating, **does the position of the kink(s) oscillate too?**
## Short answer
**NO**, the oscillation of the kink position that you see starting from an initially symmetric state is a numerical effect.
## Long Answer
We do not have analytical arguments to give a rigorous answer. 
What we can say is that, due to the analysis of [[Effective dynamics of kinks under slow POSITIVE oscillations]], that we managed to extend also to the slow oscillating limit (up to first order), the kinks should not move.
We expect that they do not move (on average) to the left or the right and additionally we expect they do not oscillate!
But this argument is valid only in the limit of slow oscillations and up to first order, so is **not valid in general! So let's make simulations!**

## Amplitude of the kink position oscillation as a function of dx

We measure the variations of the kink position by looking at the function
$$\int_{0}^L dx \frac{1}2 (u(x)+1)$$
This is a measure of the area under the +1 domain. So if the position of the kink oscillates, this integral will oscillate too.
Simulations, carried at different values of dx, show that the kink position oscillates, with an amplitude that decreases with dx. This means that the phenomena we see is a **numerical effect** due to space discretization! So **it is not a real effect.**

| dx=0.1![[Pasted image 20241126174629.png]] | dx=0.01![[Pasted image 20241126174304.png]] |
| ------------------------------------------ | ------------------------------------------- |
## Amplitude as a function of the initial displacement from the center
If the initial kink position is not the center of the box $x_{0}=L/2$ but it is slighlly displaced, we see that the amplitude of the oscillation increases with the initial displacement.
![[Pasted image 20241126174843.png]]
## Measuring the kink position by looking at the zero of $u(x)$
Also tracking the kink position in this way, leads to the same result: the amplitude of the oscillation decreases with dx, so this is a numerical effect!

| dx=0.1![[Pasted image 20241126175038.png]] | dx=0.01![[Pasted image 20241126175052.png]] |
| ------------------------------------------ | ------------------------------------------- |
