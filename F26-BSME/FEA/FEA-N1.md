

15 mins late

Chapter 10 in statics is the virtual work approach and is fundamental to FEA

Chapter 10: Method of Virtual Work

Work of a force: $W=Fd$

Mechanical efficiency is neglected

Potential Energy Approach is extracted from virtual work
Work of a spring, work of a moment

---
Virtual work method

Virtual = not real

$W=Fd$ only applies in the same direction

$dU$ = infinitesimal work of a force
$\vec{dr}$ = the incremental motion of the particle

$$dU= \vec{F}\cdot  \vec{dr}$$
$dU$ is a scalar value

algebraically: $dU=F(dr) \cos{\theta}$

Total work:
$$U=\int  \, dU =\int_{r_{1}}^{r_{2}}  \vec{F} \, d\vec{r} $$

$\vec{F}$ is the sum of all forces applied to a particle
condition for equilibrium is $F=0$


## 8-26

solve reactions of a simply supported beam using equilibrium method and virtual work method

$$\sum M_{A}=0$$
$$B_{y}(10')-20k(2')=0\to B_{y}=4kips$$
$$\sum F_{y}=0$$
$$A_{y}+B_{y}-20k=0\to A_{y}=16kips$$

equilibrium method:
for beam to be in equilibrium the following must be true
$$dU=\sum F\cdot dr=0$$
translate the beam an arbitrary amount with a slight tilt
use the displacement as dr values, should all be equal

$$dU=A_{y}\delta y_{A}+A_{x}\delta x_{A}-20k(\delta y_{C})+B_{y}\delta y_{B}=0$$

use similar triangle relation
...
$$\delta y_{c}=0.2(y_{B}-y_{A})+y_{A}=0.2y_{B}+0.8y_{A}$$
plug back into original equation

![[Pasted image 20260826193438.png|500]]


## 8-31

Check numerical answer from before 
$$\theta \approx 53.7^{\circ}$$

verify using Matlab Fzero

![[Pasted image 20260831195233.png|400]]

..





