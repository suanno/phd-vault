
As the [[Elliptic equations]] and [[Hyperbolic equations]] is labelled by considering the **highest-order derivatives** and making an analogy with the geometry of conic sections. 

$$\frac{\partial u}{\partial t} = \sum_{i,j=1}^n a_{ij} \frac{\partial^2 u}{\partial x_i \partial x_j} + \text{lower-order terms},$$
It describe the **dynamics** (towards equilibrium) of a diffusion-like process,
e.g.: Heat equation $\partial_t u = \Delta u$


### **1. Elliptic PDEs**

- **General Form**:
    

    
    where the coefficient matrix [aij][a_{ij}] is positive definite (all eigenvalues > 0).
    
- **Physical Interpretation**:
    
    - Elliptic PDEs model _steady-state_ or _equilibrium_ problems, where there is no time dependence.
    - Examples: Heat distribution in a steady state, electrostatics, incompressible fluid flow.
- **Example**:
    
    - Laplace's equation: Δu=0,or ∂2u∂x2+∂2u∂y2=0.\Delta u = 0, \quad \text{or } \frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} = 0.
    - Poisson’s equation: Δu=f(x).\Delta u = f(x).
- **Boundary Conditions**:
    
    - Typically Dirichlet (value specified) or Neumann (derivative specified).
- **Geometric Analogy**: Related to ellipses. The solution is smooth and depends on the boundary conditions of the entire domain.
    

---

### **2. Parabolic PDEs**

- **General Form**:
    
   
    
    where [aij][a_{ij}] is positive semi-definite (eigenvalues ≥0\geq 0).
    
- **Physical Interpretation**:
    
    - Parabolic PDEs model _time-dependent diffusion-like processes_, where the system evolves toward equilibrium.
    - Examples: Heat flow, diffusion of substances, and price evolution in financial models.
- **Example**:
    
    - Heat equation: ∂u∂t=αΔu,or ∂u∂t=α(∂2u∂x2+∂2u∂y2).\frac{\partial u}{\partial t} = \alpha \Delta u, \quad \text{or } \frac{\partial u}{\partial t} = \alpha \left(\frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2}\right).
- **Boundary and Initial Conditions**:
    
    - Requires initial conditions (at t=0t=0) and boundary conditions in the spatial domain.
- **Geometric Analogy**: Related to parabolas. Solutions "smooth out" over time due to the dissipative nature.
    

---

### **3. Hyperbolic PDEs**

- **General Form**:
    
    
    
    where [aij][a_{ij}] has both positive and negative eigenvalues (indefinite matrix).
    
- **Physical Interpretation**:
    
    - Hyperbolic PDEs model _wave-like_ phenomena, where information propagates at finite speeds.
    - Examples: Vibrations, sound waves, electromagnetic waves.
- **Example**:
    
    - Wave equation: ∂2u∂t2=c2Δu,or ∂2u∂t2=c2(∂2u∂x2+∂2u∂y2).\frac{\partial^2 u}{\partial t^2} = c^2 \Delta u, \quad \text{or } \frac{\partial^2 u}{\partial t^2} = c^2 \left(\frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2}\right).
- **Boundary and Initial Conditions**:
    
    - Requires both initial position and velocity conditions.
- **Geometric Analogy**: Related to hyperbolas. Solutions propagate along characteristic curves or surfaces, forming wavefronts.
    

---

### Summary Table:

|**Type**|**Form**|**Behavior**|**Example**|**Analogy**|
|---|---|---|---|---|
|**Elliptic**|No time derivative|Equilibrium (steady state)|Laplace, Poisson|Ellipses|
|**Parabolic**|First-order time derivative|Diffusion, smoothing|Heat equation|Parabolas|
|**Hyperbolic**|Second-order time derivative|Wave propagation|Wave equation|Hyperbolas|

Each type of PDE requires different mathematical techniques for analysis and has distinct implications for physical phenomena. Let me know if you'd like detailed examples or numerical methods for solving these equations!