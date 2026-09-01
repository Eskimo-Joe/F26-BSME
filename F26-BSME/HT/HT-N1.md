
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



