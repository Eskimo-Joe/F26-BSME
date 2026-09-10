
Intro session
What is heat? 
Is heat a scalar or vector? 
(vector)

class intros

The concepts are easy but the math is hard

Conduction, convection, radiation

Get the textbook

More about heat

if a cup has 90C coffee and it is not drinkable until 45C, how much heat needs to be lost and how long will it take

Thermodynamics can answer the first question
heat transfer answers the second question

## 8-26

CH1: intro and basic concepts
- Thermo review
- heat transfer mechanisms
	- conduction
	- convection
	- radiation

rate of heat transfer $\to \dot{Q}$

problems are of two types
1. rating
2. sizing

$E=U+KE+PE$
total energy is the sum of internal energy, kinetic energy, and potential energy
$e=\frac{E}{m}$

$1Btu = 1.055kJ$
$1cal = 4.1868J$

Enthalpy: $h=u+Pv$ ($\frac{kJ}{kg}$)

Specific heat: $c=\frac{\Delta E}{m \Delta T}$ ($\frac{kJ}{kg\cdot K}= \frac{kJ}{kg \cdot ^{\circ}C}$)
	at constant pressure: $c_{p}$
	at constant volume: $c_{v}$

For ideal gas: $c_{p}=c_{v}+R$
$R$: gas constant

$$du=u_{2}-u_{1}=\int _{1}^{2}  \, du=\int _{1}^2 c_{v} \, dT \approx \Delta T\cdot c_{v,avg} $$
$$dh=h_{2}-h_{1}=\int _{1}^2 \, dh=\int _{1}^2 c_{p} \, dT \approx \Delta T \cdot c_{p,avg} $$

Energy Balance (1st law of thermodynamics)
closed system:
$$Q_{in}-Q_{out}+E_{gen}=\Delta E_{thermal,system}$$
$$\Delta E_{therm}=\Delta U+\Delta KE+\Delta PE$$
KE and PE are zero for stationary systems

open system (like analyzing control volumes):
$$\dot{Q}_{in}-\dot{Q}_{out}+\dot{E}_{gen}=\dot{m}\Delta h$$

example problem:
house heating system, inefficient but simple system
resistance heating air in a duct 

![[F26-BSME/MISC/Excalidraw/Drawing 2026-08-26 11.37.02.excalidraw]]
Find: $\dot{w}_{e}$
$$\dot{Q}_{in}-\dot{Q}_{out}+\dot{E}_{gen}=\dot{m}\Delta h$$
$$0-\dot{Q}_{loss}+\dot{W}_{fan}+\dot{W}_{e}=\dot{m}c_{p,avg}\Delta T$$
$$\dot{W}_{e}=\dot{Q}_{loss}-\dot{W}_{fan}+(5^\circ C)\dot{m}c_{p,avg}$$
$$\dot{W}_{e}=250W-300W+(5C)\left( 0.6 \frac{kg}{s} \right)\left( 1.005 \frac{kJ}{kg\cdot C} \right)\left( \frac{1000J}{1kJ} \right)$$
$$\dot{W}_{e}=2965W$$

Heat Transfer Mechanisms
1. Conduction
2. Convection
3. Radiation

Conduction
if the inside of the duct wall is hot and the outside is cool, conduction is the mode of heat transferring through solids or stationary fluids

linear change across solids

Fourier's law of conduction
$$\dot{Q}_{cond}=k\frac{(T_{1}-T_{2})A}{L}\quad \left( \frac{kJ}{s} \right)$$
$k$: thermal conductivity ($\frac{W}{mK}$)
$k_{air}=0.26 \frac{W}{mK}$
$k_{diamond}=23 \frac{W}{mK}$
water and copper


## 8-31

Missed 1hr of class.. 

example problems



## 9-02

33 mins late... 

end of ch1

Chapter 2: The Conduction Equation
conductive heat transfer will be an ODE
Since heat is a vector, we will define coordinate systems
Generalized Fourier's Law
How to solve 1-D heat conduction equation

### Coordinate Systems
- rectangular ($x,y,z$)
- cylindrical ($r,\phi,z$)
- spherical ($r,\phi,\theta$)

Dimensionality of Heat Transfer 
3D transient is the hardest to solve 
transient = changes with time
steady = does not change with time

### Fourier's Law
1D:
$$\dot{Q}_{cond}=-kA \frac{dT}{dx}$$
conduction flows perpendicular to isothermal surfaces

$$\dot{Q}_{cond}=-kA \frac{dT}{dn}$$
$\vec{n}$ is the unit normal vector of the isothermal surface

$$\dot{Q}_{cond}=\dot{Q}_{x}\hat{i}+\dot{Q}_{y} \hat{j}+\dot{Q}_{z} \hat{k}$$


## 9-09


Heat generation
can be from electrical heating, nuclear reactions, solar absorption

Heat Conduction Equation (1D)

$$\dot{Q}_{cond}=\frac{kA(T_{1}-T_{2})}{L}$$
cannot determine temperature at distance and time
cannot account for heat generation

An ODE is required to determine temperatures at given locations and time

$$\dot{Q}_{cond}=-kA \frac{dT}{dx}$$
$$Q_{in}-Q_{out}+E_{gen}=\Delta E_{sys}$$
$$\dot{Q}_{in}-\dot{Q}_{out}+\dot{E}_{gen}=\frac{dE_{sys}}{dt}$$
$$\dot{Q}_{x}-\dot{Q}_{x+\Delta x}+A\Delta x \dot{e}_{gen}=\rho Vc_{p} \frac{dT}{dt}$$
$$-\frac{\dot{Q}_{x+\Delta x}-\dot{Q}_{x}}{A\Delta x}+\dot{e}_{gen}=\rho c_{p} \frac{dT}{dt}$$
by using the definition of a derivative we can sub out $\dot{Q}$

$$- \frac{1}{A} \frac{d\dot{Q}_{x}}{dx}+\dot{e}_{gen}=\rho c_{p} \frac{dT}{dt}$$
$$\frac{1}{A} \frac{d}{dx}\left(  kA \frac{dT}{dx} \right)+\dot{e}_{gen}=\rho c_{p} \frac{dT}{dt}$$
rewrite as partial derivative
$$\frac{1}{A} \frac{ \partial  }{ \partial x } \left( kA \frac{ \partial T }{ \partial x }  \right)+\dot{e}_{gen}=\rho c_{p} \frac{ \partial T }{ \partial t } $$
Heat conduction equation ^ $T(x,t)$
$$\frac{ \partial  }{ \partial x } \left( k \frac{ \partial T }{ \partial x }  \right)+ \dot{e}_{gen}=\rho c_{p} \frac{ \partial T }{ \partial t } $$
generalization to 3D
$$\frac{ \partial  }{ \partial x } \left( k \frac{ \partial T }{ \partial x }  \right)+\frac{ \partial  }{ \partial y } \left( k \frac{ \partial T }{ \partial y }  \right)+\frac{ \partial  }{ \partial z } \left( k \frac{ \partial T }{ \partial z }  \right)+ \dot{e}_{gen}=\rho c_{p} \frac{ \partial T }{ \partial t } $$

Long Cylinder
heat is only moving in radial direction, so it is a 1D heat transfer
$$\frac{1}{A} \frac{ \partial  }{ \partial r } \left( kA \frac{ \partial T }{ \partial r }  \right)+\dot{e}_{gen}=\rho c_{p} \frac{ \partial T }{ \partial t } $$
$$\frac{1}{r} \frac{ \partial  }{ \partial r } \left( kr \frac{ \partial T }{ \partial r } \right)+ \dot{e}_{gen}=\rho c_{p} \frac{dT}{dt}$$

Sphere

$$\frac{1}{r^2} \frac{ \partial  }{ \partial r } \left( kr^2 \frac{ \partial T }{ \partial r }  \right)+ \dot{e}_{gen}=\rho c_{p} \frac{ \partial T }{ \partial t } $$
the constants of area cancel out, but must put variables where they do to take the proper derivative





