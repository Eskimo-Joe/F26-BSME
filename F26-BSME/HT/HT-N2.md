
## 9-16

went over hw problem

there is variable thermal conductivity
$$\frac{d}{dx}\left( \frac{dT}{dx} \right)=0$$
solving for $\dot{Q}$ and $T(x)$ from left to right 

$$\dot{Q}_{cond}= \frac{kA(T_{1}-T_{2})}{L}$$
you cannot use this because k is dependent on temperature. You know the k value for the left and right surfaces but not throughout the conduction path

$$\int \frac{d}{dx}\left( \frac{dT}{dx} \right) \, dx =\int 0 \, dx $$
$$k \frac{dT}{dx}=C_{1}$$
$$\int k \frac{dT}{dx} \, dx =\int C_{1} \, dx $$
$$\int_{T_{1}}^{T_{2}} k(T) \, dT=\int_{0}^L C_{1} \, dx  =C_{1}L$$
$$C_{1}=\frac{1}{L}\int _{T_{1}}^{T_{2}}k(T) \, dT $$
$$\dot{Q}_{cond}=-kA \frac{dT}{dx}|_{x_{0}}=-kA \frac{C_{1}}{k}=AC_{1}$$
$$\dot{Q}_{cond}=-\frac{A}{L}\int _{T_{1}}^{T_{2}}k(T) \, dT =\frac{k_{avg}A(T_{1}-T_{2})}{L} $$
$$k_{avg}= \frac{\int _{T_{1}}^{T_{2}}k(T) \, dT }{T_{2}-T_{1}}$$
$$\dot{Q}_{cond}=\frac{k_{avg}A(T_{1}-T_{2})}{L}$$
$$k(T)=k_{0}(1+\beta T)$$
$\beta$ - temperature coefficient of thermal conductivity

$$\frac{k_{0}\beta}{2}T^2+k_{0}T+(-C_{1}x-C_{2})=0$$

...

$$T(x)=-\frac{1}{\beta}+\sqrt{ \frac{1}{\beta^2}+\frac{2}{k_{0}\beta}(C_{1}x+C_{2}) }$$

third order Dif Eq
$$y'''+(y'')^4=Tx^5$$


$$\frac{d^2y}{dx^2}-\lambda^2y=0$$
$$y(x)=C_{1}e^{\lambda x}+C_{2}e^{-\lambda x}$$

cylindrical coordinates
$$\frac{1}{r} \frac{d}{dr}\left( r \frac{dy}{dr} \right)-B^2y=0$$
$$y(r)=C_{1}I_{0}(Br)+C_{2}K_{0}(Br)$$
$I_0$ and $K_{0}$ are bessel functions
they are functions of B and r

Done with Chapter 2

there will be a hw for ch2 posted today due next wednesday Sept 23
the midterm will focus heavily on chapter 2, likely the week of Sept 28
approximately 3 questions
some will be from the homework

Chapter 3 Start
Steady Conduction

capable of solving 2D and 3D heat transfer problems

- Thermal resistance and networks
- Fin heat transfer

Thermal resistance approach
can be defined for all three modes of HT

$$\dot{Q}_{cond}=\frac{kA(T_{1}-T_{2})}{L}$$
if you think of putting a voltage across a wire, a current is created
$$I=\frac{V_{1}-V_{2}}{R_{e}}$$

temperature will correspond to voltage
heat will correspond to electrical current

conduction
$$\dot{Q}=\frac{T_{1}-T_{2}}{R_{th}}$$

$$\frac{kA(T_{1}-T_{2})}{L}=\frac{T_{1}-T_{2}}{R_{th}}$$
$$R_{th}=\frac{L}{kA}$$

Convection
$$\dot{Q}_{conv}=\frac{T_{s}-T_{\alpha}}{R_{conv}}=hA(T_{s}-T_{\alpha})$$
$$R_{conv}=\frac{1}{hA}$$

radiation
$$\dot{Q}_{rad}=\frac{T_{s}-T_{sur}}{R_{rad}}=\epsilon \sigma A_{s}(T_{s}^4-T_{sur}^4)$$
$$\dot{Q}_{rad}=\epsilon \sigma(T_{s}^2+T_{sur}^2)(T_{s}+T_{Sur})\cdot A_{s}(T_{s}-T_{sur})$$
$$\dot{Q}_{rad}=h_{rad}A_{s}(T_{s}^4-T_{sur}^4)$$
$h_{rad}$ - radiation heat transfer coefficient
$$R_{rad}=\frac{1}{h_{rad}A_{s}}$$

now u can model systems by using heat resistors as you would electrical networks

resistors in parallel, one convection and one radiation:
$$R_{comb}=\frac{1}{h_{comb}A}$$
$$\dot{Q}=\dot{Q}_{conv}+\dot{Q}_{rad}$$
$$\frac{1}{R_{comb}}=\left( \frac{1}{R_{conv}}+\frac{1}{R_{rad}} \right)^{-1}$$
$$h_{comb}A=h_{conv}A+h_{rad}A$$
$$h_{comb}=h_{conv}+h_{rad}$$
can simply be added together

starting point for next week
HT Problem like this
wall separating hot gas ($T_{h\infty}$) on left
cold gas on left ($T_{c\infty}$)

how to model with thermal resistance: literally just a convection resistor, a wall conductivity resistor, and another convection resistor

so three resistors in series
"thermal resistance network"

they add in series and in parallel! very simple


## 9-21

example problem

car driving in freezing conditions
air is -10C
windshield accumulates ice bc air has humidity
turn on the defrosters, forcing hot air onto the windshield

draw windshield as a wall
$k_{wall}=1.4 \frac{W}{mK}$
outside air $T=-10C;\quad h_{0}=200 \frac{W}{m^2K}$
Inside air $T=25C$
find minimum enthalpy of inside air so windshield doesnt ice

thickness of windshield $L=5mm$	

Although not directly stated, should know the windshield needs to be >0C to prevent ice from forming

thermal resistance network, three in series

the ends have $T_{\infty}$ for the air temperatures, then solve for thermal resistance of the two convective heat transfers and conduction of the windshield

$$R_{conv,out}=\frac{1}{h_{0}A}$$
$$R_{cond,w}=$$
$$R_{conv,in}=\frac{1}{h_{min}A}$$
u want the heat loss of the exterior to equal the heat gained from the internal convection and windshield conduction

$$\frac{T_{ice}-T_{out}}{R_{conv,1}}=\frac{T_{in}-T_{ice}}{R_{cond}+R_{conv,2}}$$
$$\dot{Q}=\frac{0-(-10C)}{R_5\times 10^{-3} \frac{K}{W}}=2000W$$
$$R_{cond}+R_{conv,2}=\frac{25C-0C}{2000W}$$
$$R_{conv,2}=\frac{25}{2000}-R_{wall}=\frac{25}{2000}-3.57\times 10^{-3} \frac{K}{W}$$
$$R_{conv,2}=8.93\times 10^{-3} \frac{K}{W}$$
$$h_{min}=\frac{1}{R_{conv,2}A}=112 \frac{W}{m^2K}$$
using $A=1m^2$ in all instances to simplify the calculation

assume steady state to solve, even though it will take time to achieve steady state

solving for the internal surface temp is not needed, but can be done easily

use the resistance network and use $\dot{Q}=\frac{\Delta T}{R}$
$T_{2}=7.14C$


we can apply the same principles to multilayer plain walls

some windshields will have a plastic layer
its conduction will add a new resistor
two contacting solids will have imperfect contact, so the resistance should be accounted for 

contact resistance
$$R_{c}\left[ \frac{Km^2}{W} \right]=R_{con}A_{c}$$
$$R_{c}=5\times 10^{-6} - 5\times 10^{-4} \frac{m^2K}{W}$$
use this form to add a resistor in your network:
$$R_{con}=\frac{R_{c}}{A_{c}}$$

## 9-23

generalized thermal resistance networks
strictly speaking, resistance method only applies to 1-D, steady, $\dot{e}_{gen}=0$

But can be extended to 2D/3D to get an approximate solution

wall that is  a sandwich
for half the length the insulation is multilayer $k_{1}$ and $k_{2}$
for half the length the insulation is $k_{3}$
not only will both halves have different conductivities and contact resistance, but the two halves will exchange heat with each other

model the multilayer as parallel resistors

1-D cylinder HT
inside: $T_{1}$
outside: $T_{2}$

$$\dot{Q}_{r}=-kA \frac{dT}{dr}$$
$$\dot{Q}_{r}=\frac{T_{1}-T_{2}}{R_{cyl}}$$
$$\int \frac{\dot{Q}_{r}}{r} \, dr=-2\pi \int _{T_{1}}^{T_{2}}  kL\, dT $$
$$\dot{Q}_{r}\ln\left( \frac{r_{2}}{r_{1}} \right)=2\pi kL(T_{1}-T_{2})$$
$$\dot{Q}_{r}=\frac{T_{1}-T_{2}}{\frac{\ln\left( \frac{r_{2}}{r_{1}} \right)}{2\pi kL}}$$
$$R_{cyl}=\frac{\ln\left( \frac{r_{2}}{r_{1}} \right)}{2\pi kL}$$

sphere
$$A=4\pi r^2$$
$$R_{sph}=\frac{r_{2}-r_{1}}{4\pi r_{1}r_{2}k}$$

example

cylinder with aluminum on bottom half, aluminum on inside of top half, copper on outside of top half
$r_{2}$ is the outside of aluminum radius
$r_{3}$ is outside of the copper
$$r_{1}=3cm;\quad r_{2}=5cm;\quad r_{3}=6cm$$
$$h_{1}=1000 \frac{W}{m^2K}$$
$$T_{\infty,1}=150C;\quad h_{2}=20 \frac{W}{m^2K}$$
$$T_{\infty,2}=25C$$
find heat loss per unit length ($\dot{Q}$)
find $\Delta T$ across the interface of the Al and Cu

steady heat transfer
2-D problem since there is not axissymetry
$\dot{e}_{gen}=0$

start by drawing resistor network
internal fluid convection to aluminum
conduction through aluminum
then two resistors in parallel to convect to the outside and contact resistance to aluminum 
the contact resistor will have another resistor 
to conduct through copper
then copper will convect

problems like this assume the outside surface is uniform temperature, even if not realistic

...
double the resistance because area is half since pipe is divided in 2


