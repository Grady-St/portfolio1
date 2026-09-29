# A6 – Design for Strength and Stiffness II

## Objective

The objective of this assignment is to develop a parametric CAD model and fully dimensioned engineering drawing of the bracket that satisfies the required strength, stiffness, and sliding-fit requirements. The design will use the results from the previous analysis to establish the governing dimensions, incorporate appropriate engineering tolerances, and document the final design using third-angle projection.


## Analyze

This is my parametrically designed solid model

https://mail.google.com/mail/u/0?ui=2&ik=d0d76599d6&attid=0.1&permmsgid=msg-a:r2364581324297823843&th=1a0eb56d435d801e&view=att&disp=safe&realattid=f_mum5l5to0&zw

This is my fully dimensioned multiview drawing in CAD with engineered tolerances.

https://mail.google.com/mail/u/0?ui=2&ik=d0d76599d6&attid=0.2&permmsgid=msg-a:r2364581324297823843&th=1a0eb56d435d801e&view=att&disp=safe&realattid=f_mum5lanr1&zw

## Reflections

a) The maximum allowable deflection was \(0.005\) in. Using the loading condition of 800 lbf and the material modulus of elasticity from the analysis, the stiffness calculation resulted in a required dimension of 0.310 in. The stress calculation only required 0.250 in, so stiffness governed the final Feature 5 dimension.  In Creo, I treated the Feature 5 dimension as a parametric dimension rather than simply modeling the part with a fixed value. The relationship can be expressed by substituting the rectangular-section equation into the deflection equation.

This showed me why a parametric model is useful for engineering design. If the load, material, allowable deflection, or another dependent dimension changes, the model can update through the relationships instead of requiring every feature to be manually edited. In the previous analysis, I also found that an error in an earlier feature could affect the later features because the bracket was analyzed sequentially.

b) For the dimension associated with the T-beam sliding interface, I used a tighter tolerance because this feature has a direct functional purpose. The bracket must fit over the specified T-beam, so the clearance between the bracket and T-beam affects whether the parts can actually assemble and slide as intended. 

Using the tightest tolerance on every dimension would unnecessarily increase manufacturing requirements. A manufacturer may need additional machining operations, tighter inspection requirements, or more precise equipment to consistently produce dimensions within a very small tolerance. Based on that tolerances should be assigned based on the function of each feature, rather than applying the smallest tolerance everywhere.

Total time spent: ~8-9 hours
