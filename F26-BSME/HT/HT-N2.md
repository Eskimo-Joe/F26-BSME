
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



