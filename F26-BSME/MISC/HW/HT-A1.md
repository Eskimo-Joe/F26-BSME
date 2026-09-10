---
class: HT
date: 2026-09-09
submitted: T
---

Problem 1
What is the importance of modeling in engineering? How are the mathematical models for engineering processes prepared?

Modeling is important because it converts a real engineering system into a simplified representation that can be analyzed, optimized, and designed safely and economically.

Engineering mathematical models are prepared by:

1. Defining the system and its boundaries.
2. Identifying relevant physical laws, such as conservation of mass, energy, and momentum.
3. Stating assumptions and simplifications.
4. Assigning material properties and boundary/initial conditions.
5. Formulating governing equations.
6. Solving and validating the model against experimental or known results.


Problem 2
Consider a 150-W incandescent lamp. The filament of the lamp is 5-cm long and has a diameter of 0.5 mm. The diameter of the glass bulb of the lamp is 8 cm. Determine the heat flux, in W/m2, (a) on the surface of the filament and (b) on the surface of the glass bulb, and (c) calculate how much it will cost per year to keep
that lamp on for eight hours a day every day if the unit cost of electricity is $0.08/kWh.

![[Pasted image 20260909090409.png|200]]

$$\dot{Q} = 150W,\quad L=0.05m,\quad d = 0.0005m$$
$$A_{filament}=\pi dL=\pi(0.0005m)(0.05m)=7.854\times 10^{-5} m^2$$
$$q_{f}''=\frac{\dot{Q}}{A_{f}}=\frac{150W}{7.854\times 10^{-5}m^2}=1.91 \times 10^6 \frac{W}{m^2}$$

$$A_{bulb}=4\pi r^2=4\pi(0.04m)^2=0.0201 m^2$$
$$q''_{b}=\frac{150W}{0.0201m^2}=7.46\times 10^3 \frac{W}{m^2}$$
$$E=(0.15kW)\left( 8 \frac{h}{day} \right)(365 days)=438kWh$$
$$ Cost = (438kWh)(0.08 $/kWh)=$35.04$$

Problem 3
A 15-cm-diameter aluminum ball is to be heated from 80◦C to an average temperature of 200◦C. Taking the average density and specific heat of aluminum in this temperature range to be ρ = 2700 kg/m3 and cp = 0.90 kJ/(kg K),  respectively, determine the amount of energy that needs to be transferred to the aluminum ball.

$$D= 0.15m,\quad T_{1}=80^{\circ}C,\quad T_{2}=200^{\circ}C$$
$$\rho= 2700 \frac{kg}{m^3},\quad c_{p}=0.9 \frac{kJ}{kg\cdot K}$$
$$V=\frac{4}{3}\pi r^3=\frac{4}{3}\pi(0.075m)^3=0.001767 m^3$$
$$m=\rho V=\left( 2700 \frac{kg}{m^3} \right)(0.001767 m^3)=4.771kg$$
$$Q=mc_{p}\Delta T=\left( 4.771 kg \right)\left( 0.9 \frac{kJ}{kg\cdot K} \right)(120K)=515kJ$$

Problem 4
In many manufacturing plants, individuals are often working around high temperature surfaces. Exposed hot surfaces that are potential for thermal burns on human skin tissue are considered to be hazards in the workplace. Metallic surface of temperature above 70◦C is considered extremely high temperature in the context of thermal burn, where skin tissue damage can occur instantaneously upon contact with the hot surface. Consider an AISI 1010 carbon steel strip 
(ρ = 7832 kg/m3) of 2 mm thick and 3 cm wide that is conveyed into a chamber to be cooled at a constant speed of 1 m/s. The steel strip enters the cooling chamber at 597◦C. Determine the amount of heat rate that needed to be removed so that the steel strip exits the chamber at 47◦C to avoid instantaneous thermal burn upon accidental contact with skin tissue. Discuss how the conveyance speed can affect the heat rate needed to be removed from the steel strip in the cooling
chamber.
![[Pasted image 20260909090547.png]]

$$\rho=7832 \frac{kg}{m^3},\quad t=0.002m,\quad w=0.03m$$
$$V=1 \frac{m}{s},\quad T_{in}=597^{\circ}C,\quad T_{out}=47^{\circ}C$$
$$c_{p}=0.434 \frac{kJ}{kg\cdot K}$$
$$A_{c}=tw=(0.002m)(0.03m)=6.0 \times 10^{-5}m^2$$
$$\dot{m}=\left( 7832 \frac{kg}{m^3} \right)(6.0 \times 10^{-5}m^2)\left( 1 \frac{m}{s} \right)=0.4699 \frac{kg}{s}$$
$$\dot{Q}=\dot{m} c_{p}(T_{in}-T_{out})=\left( 0.4699 \frac{kg}{s} \right)\left( 0.434 \frac{kJ}{kg\cdot K} \right)(597C-47C)=112kW$$


Problem 5
Air enters the duct of an air-conditioning system at 15 psia and 50◦F at a volume flow rate of 450 ft3/min. the diameter of the duct is 10 inches and heat is transferred to the air in the duct from the surroundings at a rate of 2 Btu/s. Determine (a) the velocity of the air at the duct inlet and (b) the temperature of the air at the exit.
$$P= 15psia,\quad T_{1}=50^\circ F,\quad \dot{V}=450 \frac{ft^3}{min}$$
$$D= 10in,\quad \dot{Q} = 2 \frac{Btu}{s}$$
$$T_{1}=50+459.67=509.67R$$
$$P=15 psia\left( 144 \frac{psfa}{psia} \right)=2160 \frac{lbf}{ft^3}$$
$$\rho=\frac{\left( 2160 \frac{lbf}{ft^3} \right)}{\left( 53.35 \frac{ft\cdot lbf}{R\cdot lbm} \right)(509.67R)}=0.07944 \frac{lbm}{ft^3}$$
$$A= \frac{\pi D^2}{4}=\frac{\pi\left( \frac{10}{12}ft \right)^2}{4}=0.5454ft^2$$
$$\dot{V}=\frac{450ft^3}{60s}=7.5 \frac{ft^3}{s}$$
$$V=\frac{\dot{V}}{A}=\frac{7.5 \frac{ft^3}{s}}{0.5454 ft^2}=13.75 \frac{ft}{s}$$

$$\dot{m}=\rho \dot{V}=\left( 0.07944 \frac{lbm}{ft^3} \right)\left( 7.5 \frac{ft^3}{s} \right)=0.5958 \frac{lbm}{s}$$
$$\dot{Q}=\dot{m}c_{p}(T_{2}-T_{1})$$
$$\Delta T=\frac{\left( 2 \frac{Btu}{s} \right)}{\left( 0.5958 \frac{lbm}{s} \right)\left( 0.24 \frac{Btu}{lbm\cdot R} \right)}=13.99^{\circ}F$$
$$T_{2}=T_{1}+\Delta T=50F+14F=64^\circ F$$


Problem 6
An aluminum pan whose thermal conductivity is 237 W/(m K) has a flat bottom with diameter 15 cm and thickness 0.4 cm. Heat is transferred steadily to boiling water in the pan through its bottom at a rate of 1400 W. If the inner surface of the bottom of the pan is at 105◦C, determine the temperature of the outer
surface of the bottom of the pan.

$$k=237 \frac{W}{mK},\quad D=0.15m,\quad L=0.004m$$
$$\dot{Q}=1400W,\quad T_{inner}=105^\circ C$$
$$A=\frac{\pi D^2}{4}=\frac{\pi(0.15m)^2}{4}=0.01767 m^2$$
$$\dot{Q}=kA \frac{T_{outer}-T_{inner}}{L}$$
$$\Delta T=\frac{\dot{Q}L}{kA}=\frac{(1400W)(0.004m)}{\left( 237 \frac{W}{mK} \right)(0.01767m^2)}=1.34 ^\circ C$$
$$T_{outer}=T_{inner}+ \Delta T=105C+1.34C=106.3C$$


Problem 7
The north wall of an electrically heated home is 20 ft long, 10 ft high, and 1 ft thick, and is made of brick whose thermal conductivity is k = 0.42 Btu/(h ft ◦F). On a certain winter night, the temperatures of the inner and outer surfaces of the wall are measured to be at about 62◦F and 25◦F, respectively, for a period of 8 h.
Determine (a) the rate of heat loss through the wall that night and (b) the cost of that heat loss to the home owner if the cost of electricity is $0.07/kW h.

$$L=1ft,\quad A=(20ft)(10ft)=200ft^2$$
$$k=0.42 \frac{Btu}{h\cdot ft ^\circ F}$$
$$T_{i}=62^\circ F,\quad T_{o}=25 ^\circ F$$
$$\dot{Q}=kA \frac{T_{i}-T_{o}}{L}=\frac{\left( 0.42 \frac{Btu}{h\cdot ft ^\circ F} \right)(200ft^2)(62F-25F)}{1ft}=3108 \frac{Btu}{h}$$
$$Q=\left( 3108 \frac{Btu}{h} \right)(8 h)=24864 Btu$$
$$E=\frac{24864 Btu}{3412 \frac{Btu}{kWh}}=7.287 kWh$$
$$Cost=(7.287 kWh)(0.07 $/kWh)=$0.51$$


Problem 8
Four power transistors, each dissipating 12 W, are mounted on a thin vertical aluminum plate 22 cm × 22 cm in size. The heat generated by the transistors is to be dissipated by both surfaces of the plate to the surrounding air at 25◦C, which is blown over the plate by a fan. The entire plate can be assumed to be nearly isothermal, and the exposed surface area of the transistor can be taken to be equal to its base area. If the average convection heat transfer coefficient is 25 W/(m2 K), determine the temperature of the aluminum plate. Disregard any radiation effects.

$$\dot{Q}=4\cdot 12W=48W$$
$$A_{s}=2\cdot (0.22m)(0.22m)=0.0968 m^2$$
$$\dot{Q}=hA_{s}(T_{s}-T_{\infty})\to \Delta T=\frac{\dot{Q}}{hA_{s}}$$
$$T_{s}= 25C + \frac{48W}{\left( 25 \frac{W}{m^2K} \right)(0.0968m^2)}=44.8^\circ C$$

Problem 9
Consider a sealed 20-cm-high electronic box whose base dimensions are 50 cm × 50 cm placed in a vacuum chamber. The emissivity of the outer surface of the box is 0.95. If the electronic components in the box dissipate a total of 120 W of power and the outer surface temperature of the box is not to exceed 55◦C,
determine the temperature at which the surrounding surfaces must be kept if this box is to be cooled by radiation alone. Assume the heat transfer from the bottom surface of the box to the stand to be negligible.

$$\epsilon =0.95,\quad \dot{Q}=120W,\quad T_{s}=55^\circ C$$
$$A_{t}=(0.5m)(0.5m)=0.25m^2$$
$$A_{s}=4\cdot (0.5m)(0.2m)=0.4m^2$$
$$A=0.25m^2+0.4m^2=0.65m^2$$
$$\dot{Q}=\epsilon \sigma A(T_{s}^4-T_{sur}^4)$$
$$T_{sur}=\left( T_{s}^4-\frac{\dot{Q}}{\epsilon \sigma A} \right)^{1/4}$$
$$T_{s}=55+273.15=328.15K$$
$$T_{sur}=\left[ (328.15K)^4-\frac{120W}{(0.95)\left( 5.67\times 10^{-8} \frac{W}{m^2K^4} \right)} \right]^{1/4}=300.63K$$
$$T_{sur}=300.63K-273.15=27.5^\circ C$$


Problem 10
Consider a person standing in a room at 10◦C. Determine the total rate of heat transfer from this person if the exposed surface area and the skin temperature of the person are 1.7 m2 and 32◦C, respectively, and the convection heat transfer coefficient is 5 W/(m2 K). Take the emissivity of the skin and the clothes to be 0.9,
and assume the temperature of the inner surfaces of the room to be the same as the air temperature.

$$A=1.7 m^2,\quad T_{s}=32^\circ C,\quad T_{\infty}=10^\circ C$$
$$h=5 \frac{W}{m^2K},\quad \epsilon=0.9$$
$$\dot{Q}_{conv}=hA(T_{s}-T_{\infty})=\left( 5 \frac{W}{m^2K} \right)(1.7 m^2)(22K)=187W$$
$$T_{s}=305.15\text{ K}, \quad T_{sur}=283.15K$$
$$\dot{Q}_{rad}=\epsilon \sigma A(T_{s}^4-T_{sur}^4)=(0.9)\left( 5.67\times 10^{-8} \frac{W}{m^2K^4} \right)(305.15^4-283.15^4)=194.6W$$

$$\dot{Q}_{conv}=187W,\quad \dot{Q}_{rad}=194.6W,\quad \dot{Q}_{total}=382W$$



