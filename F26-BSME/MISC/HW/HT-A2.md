---
class: HT
date: 2026-09-23
submitted: T
---

Problem 1
Consider an egg being cooked in boiling water in a pan. Would you model the heat transfer to the egg as one-, two-, or three-dimensional? Would the heat transfer be steady or transient? Also, which coordinate system would you use to solve this problem, and where would you please the origin? Explain.

An egg being cooked in a would be a 3 dimensional problem because the egg's surface is a spheroid. It sounds like not the whole egg is submerged into the boiling water, so it could not be considered a unidimensional wall. If you consider it spherical coordinates with the origin in the geometric center, you will see that heat will flow across the egg in the radial and both angular coordinates.


Problem 2
Consider a medium in which the heat conduction equation is given in its simplest form as
$$\frac{1}{r} \frac{d}{dr}\left( rk \frac{dT}{dr} \right)+\dot{e}_{gen}=0$$
(a) Is heat transfer steady or transient?
	It must be steady heat transfer because there is no time variable. 
(b) Is heat transfer one-, two-, or three-dimensional?
	Heat transfer is one-dimensional since only one coordinate is involved (r). 
(c) Is there heat generation in the medium?
	Yes, the variable $\dot{e}_{gen}$ represents the heat generated.
(d) Is the thermal conductivity of the medium constant or variable?
	The thermal conductivity is variable, as the conductivity is within the derivative with respect to $r$. 

Problem 3
Starting with an energy balance on a ring-shaped volume element, derive the two-dimensional steady heat conduction equation in cylindrical coordinates for T (r, z) for the case of constant thermal conductivity and no heat generation.

![[Pasted image 20260922210724.png]]

$$\dot{Q}_{r}-\dot{Q}_{r+dr}+\dot{Q}_{z}-\dot{Q}_{z+dz}=0$$
$$\dot{Q}_{r}=-k(2\pi r\,dz) \frac{ \partial T }{ \partial r } $$
$$\dot{Q}_{z}=-k(2\pi r\,dr)\frac{ \partial T }{ \partial z } $$
$$\frac{1}{r} \frac{ \partial  }{ \partial r } \left( r \frac{ \partial T }{ \partial r }  \right)+ \frac{ \partial ^2T }{ \partial z^2 }=0 $$


Problem 4
Consider the East wall of a house that has a thickness of L. The outer surface of the wall exchanges heat by both convection and radiation. The interior of the house is maintained at T∞1, while the ambient air temperature outside remains at T∞2. the sky, the ground, and the surfaces of the surrounding structures at this
location can be modeled as a surface at an effective temperature of Tsky for radiation exchanges on the outer surface. The radiation exchange between the inner surface of the wall and the surfaces of the walls, floor, and ceiling it faces is negligible. The convection heat transfer coefficients on the inner and outer surfaces of the wall are h1 and h2, respectively. The thermal conductivity of the wall material is k and the emissivity of the outer surface is ε2. Assuming the heat transfer through the wall to be steady and one-dimensional, express the mathematical formulation (the differential equation and the boundary and initial conditions) of this heat conduction problem. Do not solve.

![[Pasted image 20260922210816.png|300]]

thermal resistance of interior convection, and conduction from 0 to L
$$R_{conv,1}= \frac{1}{h_{1}A};\quad R_{cond}=\frac{L}{kA}$$
thermal resistance of exterior radiation
$$R_{rad}=\frac{1}{A\epsilon _{2}\sigma(T_{L}^2+T_{sky}^2)(T_{L}+T_{sky})}$$
thermal resistance of the exterior convection
$$R_{conv,out}=\frac{1}{h_{2}A}$$
energy balance of the exterior surface
$$\dot{Q}_{conv,1}+\dot{Q}_{cond}=\dot{Q}_{rad}+\dot{Q}_{conv,2}$$
$$h_{1}A(T_{0}-T_{\infty_{1}})+kA\frac{T_{L}-T_{0}}{L}=A\epsilon_{2}\sigma(T_{sky}-T_{L})(T_{L}^2+T_{sky}^2)(T_{L}+T_{sky})+h_{2}A(T_{\infty_{2}}-T_{L})$$

Problem 5
A spherical metal ball of radius ro is heated in an oven to a temperature of Ti throughout and is then taken out of the oven and dropped into a large body of water at T∞ where it is cooled by convection with an average convection heat transfer coefficient of h. Assuming constant thermal conductivity and transient one-dimensional heat transfer, express the mathematical formulation (the differential equation and the boundary and initial conditions) of this heat conduction problem. Do not solve.

$$T=T(r,t)$$
governing equation:
$$\frac{1}{r^2} \frac{ \partial  }{ \partial r } \left( r^2 \frac{ \partial T }{ \partial r }  \right)= \frac{\rho c_{p}}{k} \frac{ \partial T }{ \partial t } $$
$$0<r<r_{0}$$
Symmetry at the center
$$\frac{ \partial T }{ \partial r } |_{r=0}=0$$
fluid boundary condition
$$-k \frac{ \partial T }{ \partial r }|_{r=r_{0}} =h(T(r_{0},t)-T_{\infty})$$
initial temperature
$$T(r,0)=T_{i}$$


Problem 6
The outer surface of an engine is situated in a place where oil leakage can occur. Some oils have autoignition temperatures of approximately above 250◦C. When oil comes in contact with a hot engine surface that has a higher temperature than its autoignition temperature, the oil can ignite spontaneously. Treating the engine housing as a plane wall, the inner surface (x = 0) is subjected to 6 kW/m2 of heat. The engine housing (k = 13.5 W/(m K)) has a thickness of 1 cm, and the outer surface (x = L) is exposed to an environment where the ambient air is 35◦C with a convection heat transfer coefficient of 20 W/(m2 K). To prevent fire hazard in the event the leaked oil comes in contact with the hot engine surface, the temperature of the engine surface should be kept below 200◦C. Determine the variation of temperature in the engine housing and the temperatures of the inner and outer surface. Is the outer surface temperature of the engine below the safe
temperature?

![[Pasted image 20260922210843.png]]

$$q_{0}''=6000 \frac{W}{m^2},\, k=13.5 \frac{W}{mK},\, L=0.01m$$
$$h=20 \frac{W}{m^2K},\,T_{\infty}=35^{\circ}C$$
governing equation:
$$\frac{d^2T}{dx^2}=0$$
$$-k \frac{dT}{dx}=q_{0}''$$
$$\frac{dT}{dx}=- \frac{q_{0}''}{k}$$
$$T(x)=C_{1}-\frac{q_{0}''}{k}x$$
outer surface boundary condition
$$q_{0}''=h(T(L)-T_{\infty})$$
$$T(L)=T_{\infty}+\frac{q_{0}''}{h}=35C+\frac{6000 \frac{W}{m^2}}{20 \frac{W}{m^2K}}=335^\circ C$$
$$T(x)=T(L)+\frac{q_{0}''}{k}(L-x)=335C+\frac{6000}{13.5}(0.01-x)$$
$$T(0)=335C+\frac{6000(0.01)}{13.5}=339.4C$$
The outer surface of the engine is too hot and is a fire risk. 


Problem 7
Consider a steam pipe of length L = 30 ft, inner radius r1 = 2 in, outer radius r2 = 2.4 in, and thermal conductivity k = 7.2 Btu/(h ft ◦F). Steam is flowing through the pipe at an average temperature of 300◦F, and the average convection heat transfer coefficient on the inner surface is given to be h = 12.5 Btu/(h ft2 ◦F). If
the average temperature on the outer surfaces of the pipe is T2 = 175◦F, (a) express the differential equation and the boundary conditions for steady one-dimensional heat conduction through the pipe, (b) obtain a relation for the variation of temperature in the pipe by solving the differential equation, and (c) evaluate the rate of heat loss from the steam through the pipe.

![[Pasted image 20260922211007.png]]

$$L=30ft,\,r_{1}=2in=\frac{1}{6}ft$$
$$r_{2}=2.4in=0.2ft$$
$$k=7.2 \frac{Btu}{h\,ft\,^\circ F}$$
$$h=12.5 \frac{Btu}{h\,ft^2\,^\circ F}$$
$$T_{\infty}=300 ^\circ F,\quad T(r_{2})= 175 ^\circ F$$
cylindrical coordinates, steady heat
$$\frac{1}{r} \frac{d}{dr}\left( r \frac{dT}{dr} \right)=0$$
$$-k \frac{dT}{dr}|_{r=r_{1}}=h[T_{\infty}-T(r_{1})]$$
$$T(r_{2})=T_{2}=175^\circ F$$
$$T(r)=T_{2}$$
$$T=C_{1}\ln r+C_{2}$$
$$T(r)=T_{2}+C\ln\left( \frac{r_{2}}{r} \right)$$
$$T(r_{1})=T_{1}=T_{2}+C\ln\left( \frac{r_{2}}{r_{1}} \right)$$
$$C=\frac{h(T_{\infty}-T_{2})}{\frac{k}{r_{1}}+h\ln \left( \frac{r_{2}}{r_{1}} \right)}=\frac{12.5(300-175)}{\frac{7.2}{\frac{1}{6}}+12.5 \ln(1.2)}=34.36^\circ F$$
$$T(r)=175+34.36 \ln\left( \frac{0.2}{r} \right)$$
$$T(r_{1})=175+34.36 \ln\left( \frac{0.2}{\frac{1}{6}} \right)=181.3^\circ F$$
$$\dot{Q}=2\pi L k C$$
$$\dot{Q}=2\pi(30ft)\left( 7.2 \frac{Btu}{hft^\circ F} \right)(34.36)=4.66\times 10^4 \frac{Btu}{h}$$


Problem 8
Consider a large plane wall of thickness L = 0.05 m. The wall surface at x = 0 is insulated, while the surface at x = L is maintained at a temperature of 30◦C. The thermal conductivity of the wall is k = 30 W/(m K), and the heat is generated in the wall at a rate of ˙egen = ˙e0e−0.5x/L W/m3 where ˙e0 = 8 × 106 W/m3. Assuming steady one-dimensional heat transfer, (a) express the differential equation and the boundary conditions for heat conduction through the wall, (b) obtain a relation for the variation of temperature in the wall by solving the differential equation, and (c) determine the temperature of the insulated surface of the wall.

$$L=0.05m,\quad k=30 \frac{W}{(mK)}$$
$$\dot{e}_{gen}=\dot{e}_{0}e^{-0.5x/L}$$
$$\dot{e}_{0}=8\times 10^6 \frac{W}{m^2}$$
$$T(L)=30^\circ C$$
$$\frac{d}{dx}\left( k \frac{dT}{dx} \right)+\dot{e}_{0}e^{-0.5x/L}=0$$
$$k \frac{d^2T}{dx^2}+\dot{e}_{0}e^{-0.5x/L}=0$$
$$\frac{dT}{dx}|_{x=0}=0$$
$$T(L)=30^\circ C$$
$$\frac{dT}{dx}=- \frac{2L\dot{e}_{0}}{k}(1-e^{-x/2L})$$
$$T(x)=C_{2}- \frac{2L\dot{e}_{0}}{k}[x-2L(1-e^{-x/2L})]$$
$$T(L)=30^\circ C$$
$$T(x)=30+ \frac{2L\dot{e}_{0}}{k}[L-2L(1-e^{-0.5})-x+2L(1-e^{-x/2L})]$$
$x=0$
$$T(0)=30+ \frac{2L\dot{e}_{0}}{k}[L-2L(1-e^{-0.5})]=314.1^\circ C$$

Problem 9
A cylindrical nuclear fuel rod of 1 cm in diameter is encased in a concentric tube of 2 cm in diameter, where cooling water flows through the annular region between the fuel rod (k = 30 W/(m K)) and the concentric tube. Heat is generated uniformly in the rod at a rate of 50 MW/m3. The convection heat transfer coefficient 3 for the concentric tube surface is 2000 W/(m2 K). If the surface temperature of the concentric tube is 40◦C, determine the average temperature of the cooling water. Can one use the given information to determine the surface temperature of the fuel rod? Explain.

![[Pasted image 20260922211110.png]]

$$D_{1}=1cm;\quad D_{2}=2cm$$
$$r_{1}=0.005m;\quad r_{2}=0.01m$$
$$\dot{e}_{gen}=50 \times 10^6 \frac{W}{m^3}$$
$$h_{2}=2000 \frac{W}{m^2K}$$
$$T_{s}=40^\circ C$$
$$\dot{Q}'=\dot{e}_{gen}\pi r_{1}^2$$
$$q_{2}''=\frac{\dot{Q}'}{2\pi r_{2}}=\frac{\dot{e}_{gen}r_{1}^2}{2r_{2}}=\frac{(50\times 10^6)(0.005)^2}{2(0.01)}=62500 \frac{W}{m^2}$$
$$q_{2}''=h_{2}(T_{s}-T_{\infty})$$
$$T_{\infty}=T_{s}-\frac{q_{2}''}{h_{2}}=40-\frac{62500}{2000}=8.75^\circ C$$

Problem 10
A circular metal pipe has a wall thickness of 10 mm and an inner diameter of 10 cm. The pipe’s outer surface is subjected to a uniform heat flux of 5 kW/m2 and has a temperature of 500◦C. The metal pipe has a variable thermal conductivity given as k(T ) = k0 (1 +β T ), where k0 = 7.5 W/(m K), β = 0.0012 K−1, and T is in
K. Determine the inner surface temperature of the pipe.

![[Pasted image 20260922211140.png]]

$$r_{1}=0.05m;\quad r_{2}=0.06m$$
$$q''=5000 \frac{W}{m^2}$$
$$T_{2}=500^\circ C=773.15K$$
$$k(T)=k_{0}(1+\beta T)$$
$$k_{0}=7.5 \frac{W}{mK};\quad \beta=0.0012 K^{-1}$$
$$-k(T) \frac{dT}{dr}=- \frac{q''r_{2}}{r}$$
$$k_{0}(1+\beta T)dT=q''r_{2}\ln\left( \frac{r_{2}}{r_{1}} \right)$$
$$k_{0}\left[ (T_{2}-T_{1})+ \frac{\beta}{2}(T^2_{2}-T^2_{1}) \right]=q''r_{2}\ln\left( \frac{r_{2}}{r_{1}} \right)$$
$$7.5\left[ (773.15-T_{1})+\frac{0.0012}{2}(773.15^2-T_{1}^2) \right]=5000(0.06)\ln\left( \frac{0.06}{0.05} \right)$$
$$T_{1}=769.36K=496.2^\circ C$$



