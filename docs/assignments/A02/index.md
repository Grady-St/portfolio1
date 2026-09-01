# Project A2 – Truss Stress Analysis


## Objective

The purpose of this project was to design and analyze a lightweight planar truss capable of supporting two downward loads while meeting specified geometric, strength, and safety-factor requirements. The truss was developed using A500 structural steel and analyzed using equilibrium equations and the method of joints. The design process included selecting the truss geometry, determining support reactions, calculating internal member forces, sizing the truss members, scaling the required pin dimensions, estimating the total weight, and comparing the analytical results with a CAD model.

A primary objective of this project was to document the engineering process rather than only present the completed design. Each major design decision is supported by calculations, free-body diagrams, and material properties.


## Analyze

I have chose my parameter	values and they are listed below 
Applied load at C is P = 25 kN,
Applied load at D	is P = 25 kN,
Horizontal spacing: a = 0.40 m,
Vertical spacing: b = 0.30 m, 
Truss material: A500 Structural Steel,
Yield strength used: 46 ksi,
Member safety factor: N = 3.5,
Pin material: Cold rolled steel,
Pin shear strength: 170 ksi,
Pin safety factor: 4

<img width="560" height="534" alt="Screenshot 2026-08-31 at 6 04 46 PM" src="https://github.com/user-attachments/assets/2b2f621b-ffd6-49f0-868f-66f5ee7eec2b" />

Truss Geometry and X brace Confg.

The final truss design uses two diagonal members to create an X-braced configuration. The diagonal members extend from C to A and from D to B. The two diagonal members cross at the center of the truss but are not connected to each other at the crossing point.

I made this decision so the truss could be analyzed so all unknown support reactions and internal forces can be completely calculated using the method of joints and equation of equilibriums. If the crossing location were converted into an additional pinned joint, the number of members and unknown forces would change and a more advanced analysis method could be required.


<img width="716" height="371" alt="Screenshot 2026-08-31 at 9 24 03 PM" src="https://github.com/user-attachments/assets/481cf25b-66bb-4df3-9486-0940d3b15ec8" />

Pictured here is the free body diagram of joints C and D



<img width="716" height="550" alt="Screenshot 2026-08-31 at 9 26 08 PM" src="https://github.com/user-attachments/assets/d4f36d9a-2e13-4e88-8ce5-c9afd703e1a5" />

For these calculations, the two diagonal members are assumed to cross without being pinned together at the intersection. The intersection is simply where the members pass each other geometrically. If you connect the two diagonal members with an additional pin at the center, the truss becomes a different structural model and the internal force calculations would need to be changed.

<img width="561" height="507" alt="Screenshot 2026-08-31 at 10 01 41 PM" src="https://github.com/user-attachments/assets/6eb7644e-3b2e-4e0a-ab5c-a66e49cec492" />

<img width="561" height="507" alt="Screenshot 2026-08-31 at 10 45 46 PM" src="https://github.com/user-attachments/assets/d21edcd0-b4e8-49a7-97bb-a0552ff1e8fb" />

The required member area was determined using the material yield strength (1333.33) and the specified safety factor (3.5) . The largest force must first be converted to kips which I did by multiplying the value in kN by 0.2248. After solving every truss member must have a cross-sectional area of at least 2.281 in^2

---

# Pin Design 
3) The objective is to determine the cross-sectional area of the connecting pins which are made of hardened tool steel with a yield shear strength of 170 ksi and a density of 0.278 lb/in3.

Known/Given:
P=25kN for each downward load

a=0.40m

b=0.30m

Support Reactions:

Ay=p=25kN

By=P=25kN

Ax=0

Pin material: Cold rolled steel

Shear strength: τy=170 ksi

Density: p=0.278 lb/in^3

Single shear design with a safety factor of 4

Unkown:

Minimum cross sectional area of pins

Pin diameter

Approximate weight

<img width="561" height="735" alt="Screenshot 2026-08-31 at 11 25 38 PM" src="https://github.com/user-attachments/assets/ef958c34-9b42-4142-a3d2-e18f8552aa12" />

Free-Body Diagram and Maximum Pin Load

The pin free-body diagram was based on the largest support reaction in the truss. Since both support reactions were 25 kN, the maximum shear force used for the pin design was 25 kN. Designing for this maximum load ensures that the pins can safely withstand the most critical loading condition.

Symbolic Solution for Minimum Cross-Sectional Area

The shear stress in the pin is calculated by dividing the applied force by the pin's cross-sectional area. The allowable shear stress was found by dividing the material's yield shear strength by the safety factor. Solving the resulting equation gives the minimum required pin area:

Numerical Solution for Cross-Sectional Area

Substituting the maximum load, safety factor, and material strength produced a minimum required area of 0.588 in². Using the area equation for a circular cross section resulted in a minimum diameter of 0.866 in. A standard pin diameter of 0.875 in was selected because it exceeds the minimum required size.

Approximate Combined Weight of the Pins

Each pin was modeled as a solid cylinder with a diameter of 0.875 in and a length of 11.81 in. The calculated weight of one pin was approximately 1.97 lb. Since four pins are used at joints A, B, C, and D, the estimated combined weight is 7.88 lb.


## 5) Engineering Lessons Learned

Through this project, I learned that designing a truss requires more than simply calculating whether the members can carry an applied load. I learned how to use the yield strength of a material and a required safety factor to determine the minimum cross-sectional area needed for the truss members and connecting pins. Comparing the internal forces and resulting stresses to the allowable material strength showed me how engineering calculations directly influence physical design decisions.

I also learned about common truss design failures, including member yielding, pin shear failure, and buckling of members in compression. A member may have sufficient material strength but still fail through buckling if its geometry and unsupported length are not considered. This project demonstrated why both the forces in individual members and the type of loading—tension or compression—must be evaluated before selecting dimensions.

Another important lesson was the value of verifying analytical calculations with a CAD model. Hand calculations provide the required dimensions and predicted weight, while the CAD model helps identify potential issues with member intersections, pin placement, and overall geometry. Comparing these results helped me understand that an engineering design should be evaluated from multiple perspectives rather than relying on a single calculation.


