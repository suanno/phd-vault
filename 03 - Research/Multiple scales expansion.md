The **multiple-scale expansion** is a _perturbative_ approach to study the dynamics. 
## Idea
The dynamics of the system is the **einsemble of many process** that in principle may me **characterized by different time scales $\tau_i$** (some processes can be faster than others). So you can introduce some **new time variables** $t_i$, such that
$$\delta t_i \sim 1 \iff \delta t \sim \tau_i$$
where $\tau_{i}$ is the **time-scale** of one (ore more) processes.
In this way, you ==hope to capture== the description of each process occurring with a timescale $\tau_i$, **inside the dependence** of the state $m(\mathbf{x},t_1,t_2,...)$ **on $t_i$** (within a differential equation with $\partial_{t_{i}}m$). The new variables $\{t_i\}$ will be **treated as independent** (even if they aren't) variables and we chose to define them like this (this is the most natural way of considering timescales of **different order**)
$$\dots, t_{-1}=\epsilon^{-1}t, t_0 = t, t_1 = \epsilon t, t_2 = \epsilon^2 t, ...$$
as we threat them as independent variables, it follows that
$$
    \partial_t = \dots + \epsilon^{-1}\partial_{t_{-1}} + \partial_{t_0} + \epsilon\partial_{t_1} + \epsilon^2\partial_{t_2} + \dots
$$

#### What is $\epsilon$ ?
Within this analytical approach, **the powers of $\epsilon$ represent the time-scales we are considering**. It is important to properly choose its value as, within this approach, **we will capture (only) phenomenas occurring at those time-scales.**
In the system, there is an **intrinsic time-scale** $\tau_{linear}$ (see [[tau_linear|here]]) and, by introducing temporal oscillations of C, we introduce a new time-scale $\tau_{C}$ that is the period of the oscillation, if the oscillation is periodic.
As a consequence, it comes natural to look at phenomenas occurring at timescales that are powers of
$$\epsilon=\frac{\tau_{linear}}{\tau_{C}}\quad\text{or}\quad \epsilon=\frac{\tau_{C}}{\tau_{linear}}$$
#### Example: C(t) oscillating around 1
If C(t) oscillates around the value 1 ($\bar{C}=1$) then $\tau_{C}\sim 1$ and so $\epsilon \sim \tau_{C}^{-1}$.
ThenC
- The variable $t_{0}$ will describle the process occurring at the intrinsic time-scale as $\tau_{linear}\sim 1$ and $t_{0}= t = \frac{t}{1}$
- The variable $t_{1}$ will describe processes occurring at the time-scale of C(t)'s oscillations, as $\tau_{C}\sim \epsilon$ and $t_{1} = \epsilon t$.
Then, there could be processes occurring at different timescales that would be captured by the higher order variables.

# ==What if $\tau_{linear}$ is NOT of order 1?==
It is not clear to me how to generalize, because it makes no sense to look at processes occurrinf at the timescales 1 and $\frac{\tau_{linear}}{\tau_{C}}$ **if we expect some processes occurring at the timescales $\tau_{linear}$ and $\tau_{C}$**.
It is important if we want to explore what happens when $C(t)^{-1}\rightarrow \infty$.