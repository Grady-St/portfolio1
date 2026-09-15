# A4 – Motor Mount

## Objective
The objective of this project is to design and create a 3D CAD model of a motor mount that attaches a 24 V DC gear motor to a rigid wall while meeting strength and deflection requirements. Withstand the 300 N applied load with a safety factor of 3 while keeping the maximum deflection below 0.30 mm. Beam-bending equations will be used to determine the required geometry for the motor and wall attachment features, and the final design will be modeled in Creo with appropriate clearance holes and stiffness features.

## Analyze

<img width="585" height="769" alt="Screenshot 2026-09-14 at 11 09 27 PM" src="https://github.com/user-attachments/assets/81485ab4-cc1b-4aa6-abcb-73e96b316e33" />

I first identified the known values needed for the analysis, including the 300 N applied load, safety factor of 3, PETG material properties, beam lengths, and maximum allowable deflection. The main unknown I needed to determine was the required thickness of each feature.
Then I created a free-body diagram by simplifying each feature as a cantilever beam. I included the 300 N force at the free end and the reaction force and moment at the fixed wall. This allowed me to determine the maximum bending moment acting on each feature. For the beam-bending equations I used a rectangular cross section to calculate the bending stress and deflection. I calculated the moment of inertia using \(I=bt^3/12\), then used the stress and cantilever deflection equations to solve symbolically for the required thickness.


<img width="585" height="410" alt="Screenshot 2026-09-14 at 11 12 59 PM" src="https://github.com/user-attachments/assets/974a6d12-e874-43dd-b9f5-06e30b2b0815" />

I substituted the known values into the equations and calculated the minimum thickness required for both yield strength and deflection. The deflection requirement controlled the design, so I selected a thickness slightly larger than the calculated minimum to provide additional stiffness.


<img width="585" height="310" alt="Screenshot 2026-09-14 at 11 15 15 PM" src="https://github.com/user-attachments/assets/46e80da8-c994-4dcd-814a-037a85af7a4d" />

For the second feature, I followed the same process but used the dimensions of the wall-mounted section and I treated the rigid wall as the fixed support, calculated the bending stress and deflection, and selected a final thickness that allowed both the strength and deflection requirements.


<img width="585" height="569" alt="Screenshot 2026-09-14 at 11 19 54 PM" src="https://github.com/user-attachments/assets/8ecc7368-7d8b-4b1e-a09f-8a7d057d605f" />

I then used Creo to create the final motor mount based on the calculated dimensions. I added the motor mounting features, wall-mounting holes, and triangular sections to increase the stiffness of the mount. I also included the required 3.4 mm clearance holes for the mounting bolts and used parametric dimensions so the model could be adjusted if necessary.


<img width="1017" height="717" alt="Screenshot 2026-09-14 210941" src="https://github.com/user-attachments/assets/96445b44-54eb-4858-91e6-e2503ef9c9e5" />


<img width="1048" height="768" alt="Screenshot 2026-09-14 194932" src="https://github.com/user-attachments/assets/6bf724e4-5a31-491d-904c-d0ec08a77541" />



<img width="1157" height="750" alt="Screenshot 2026-09-14 194901" src="https://github.com/user-attachments/assets/234e02e0-272f-4314-8416-9723a68d502e" />


<img width="1041" height="722" alt="Screenshot 2026-09-14 194837" src="https://github.com/user-attachments/assets/987480f7-f68b-46b3-b8b7-af0bb5cdaf25" />

CREO file

[motormount.prt.zip](https://github.com/user-attachments/files/32221675/motormount.prt.zip)


The motor mount was designed using PETG and modeled as a combination of cantilever beam sections. The thicknesses of the two primary features were selected based on both bending stress and maximum deflection. The deflection requirement controlled the final thickness because it required a larger cross section than the strength calculation. Triangular sections were added between the base and vertical motor plate to increase stiffness and reduce bending deflection. Clearance holes were included for the wall-mounting bolts as specified in the assignment (3.4mm).

Final dimensions:

length	50 mm, 
width	60 mm, 
thickness	20 mm, 
length	50 mm, 
width	80 mm, 
thickness	18 mm, 
Wall bolt clearance holes	Ø3.4 mm, 
Material	PETG, 
Applied load	300 N, 
Safety factor	3, 
Maximum allowed deflection	0.30 mm, 


Through this project, I learned how changing the geometry of a part affects both its strength and stiffness. I found that the deflection requirement required a thicker section than the yield-strength calculation, which showed me that a design can meet its strength requirement while still needing additional material to control deformation.
