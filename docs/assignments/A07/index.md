# A7 – FEA ON BRACKET

Overview

The purpose of this project was to improve the bracket developed for Assignment A5 by using finite element analysis (FEA). The design was evaluated using maximum stress, maximum deflection, and safety factor. Three outer design iterations were completed, with an inner validation loop in each iteration. The goal was to bring the results within a 7% difference between mesh refinements, or to stop after three attempts.

# Analyze Design 1
<img width="406" height="221" alt="Screenshot 2026-10-27 at 12 55 36 AM" src="https://github.com/user-attachments/assets/95f61702-2344-4597-ba0c-8a9ab738b11b" />

This is my redesigned bracket slighly tweaked from last time

Outer Loop – Initial Model

I began with the nylon bracket created for Assignment A5. To prepare it for analysis, I applied a 500 lbf load to the cylindrical extrusion and fixed the two upper inside surfaces that rest against the T-beam in operation. I kept these loading and support conditions unchanged for all three design iterations.

Inner Loop – Mesh Validation

I first solved the model using a coarse mesh, then repeated the analysis with medium and fine meshes. I compared the results by calculating the percentage difference between consecutive mesh levels. Only the deflection results met the 7% target, so the first iteration provided direction for revising the geometry.

Mesh Results
<img width="1203" height="208" alt="Screenshot 2026-10-27 at 12 58 52 AM" src="https://github.com/user-attachments/assets/56328e6c-37fc-40bc-9064-2f076f168cb0" />

# Analyze Design 2
<img width="450" height="293" alt="Screenshot 2026-10-27 at 1 02 04 AM" src="https://github.com/user-attachments/assets/6493dd29-0d67-4699-bd11-19db51287513" />

For the second design, I added a second support to the cylindrical feature, positioned symmetrically opposite the existing rear support. I also extended the cylindrical extrusion across the full bracket length. This change was intended to reduce the stress concentrated in the cylinder's rear brace. The load and fixed constraints were not changed.

I repeated the coarse-, medium-, and fine-mesh simulations and compared the resulting values. Stress and safety factor still showed differences larger than the target, although deflection was within the 7% range. The highest stress remained near the joints between the cylindrical braces and the bracket frame that fits over the T-beam.

Mesh Results
<img width="968" height="162" alt="Screenshot 2026-10-27 at 1 19 53 AM" src="https://github.com/user-attachments/assets/37660628-e15d-4e7c-916e-94eb99222c70" />

Lessons Learned

This project showed me how strongly mesh refinement can affect finite element results. In these simulations, smaller elements generally produced higher maximum-stress and deflection values, while the calculated safety factor decreased. Comparing coarse, medium, and fine meshes helped me understand why mesh convergence should be checked before using results to make design decisions. I also gained experience applying FEA results to guide successive geometry changes, including adding support features and diagonal bracing.

Approximate time spent on the project: 8 hours.

Comparison Summary
<img width="728" height="162" alt="Screenshot 2026-10-27 at 1 21 44 AM" src="https://github.com/user-attachments/assets/f6481eff-52f5-4040-819f-a52ad4ff5ddc" />
