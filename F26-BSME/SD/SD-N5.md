
drawing of a shaft driven by a pulley
converted to a structural diagram

SW is just CAD, not acceptable for analysis
step by step tutorial of using ansys 

belts have tension that pull on the pulley
the pulley will spin when the belt has a different tension on each side
there needs to be a net moment about the pulley to spin it
same with chain drives and other drives
$$\tau_{transmission}=R_{pulley}(T_{2}-T_{1})$$
structural load is sum of tensions
torque on the pulley is difference of tensions

now learn how to calculate stresses and strains

start with solving reaction forces
draw shear-force and bending moment diagrams
find maximum stress

$$\sigma_{max}=\sigma_{shear}+\sigma _{bending}$$
$$\sigma_{max}=\frac{P}{A}+\frac{Mc}{I}$$
focus on material failure 

export CAD assemblies as IGS format

open Ansys workbench
drag in your analysis into the whitespace
import engineering materials 
import geometry
edit the model, define materials, define contacts, and define mesh parameters
- contact typed are important for the accuracy of results
	- bonded contacts
	- rough
	- frictionless
	- friction
	- etc
define the boundary conditions and loads
solve the system
can view results and apply scales

$$M=\frac{PL}{4}=\frac{(100N)(90mm)}{4}=2,250Nmm$$
$$I=\frac{\pi}{64}(d_{0}^4-d_{i}^4)=\frac{\pi}{64}(20^4-18^4)=2700.98mm^4$$
$$\sigma_{b}=\frac{(2250N)(10mm)}{\frac{\pi}{64}(20^4-18^4)}=8.33 \frac{N}{mm}$$


Find principle stresses via Mohrs circle
Also solve for von-mises stresses for maximum stresses
failure theory can be shear or tension
more advanced can use fatigue, etc



