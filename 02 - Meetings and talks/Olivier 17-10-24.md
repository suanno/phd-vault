# 1D simulations of 2 isolated kinks: plot d v.s. log(tc-t)
- Make simulations with the same parameters $\bar{C},$ A, T but increasing the initial distance d0. Check if the curves overlap or not.
- An eventual mismatch between the curves could be explained by the fact that, at the time of the annhilation of the kinks, the phase of C(t) (e.g. C(t) has reach a maxima, a minima or a zero) could be different.
- Plot the variation of d(t) during each period, as a function of the (average value) of the distance in that period.

# Phase transition between periodic and coarsening state
- Check, both in 1D and 2D simulation of the TDGL eq., if there is a critical value of $\bar{C}>0$ (call it $C^*(A,T)$) such that if
$$C(t) = \bar{C}+A\sin(2\pi t/T)\quad\text{with $A > \bar{C}$}$$
    

then 
$$if\quad\bar{C}<C^*\text{ the state is periodic (in time)}$$
$$if\quad\bar{C}>C^*\text{ the state coarsens}$$

check that, by
- keeping A, T fixed
- changing C **step-wisely** (like A. Onuki did, but he worked with the Model B not Model A).
- monitor <q^2> and the structure factor 

Notice: we expect that the time of decay of the kinks during the C<0 timespan, is associated with the lowest value of $C$ that is $\bar{C}-A$. So this timescale depends both on $\bar{C}$ and A.


- Compute the structure factor $S(q)$ in TDGL 1D and 2D.
- Notice that $S(q=0) = \int dx e^{-iqx}<u(r)u(0)>|_{q=0}$ is the average

# Double quench in a conservative system (Model B)
The mass conservation of a domain, coupled with the change of the stable uniform states, can be matched by the emergence of smaller domains inside the pre-existing ones.
