# CSE 5280 — Building Evacuation Simulation  
Nick Speranza

This project studies multi-agent evacuation inside a three-floor building using continuous cost-function minimization.

Agents move through the environment using gradient-based optimization on a shared objective containing:

- staged goal attraction  
- wall avoidance  
- surface-adherence terms  
- temporal smoothness  
- crowd repulsion  

No discrete collision checking, explicit path planning, or rule-based floor switching is used.  
Agents descend through ramps and evacuate through ground-floor exits as a result of the cost landscape alone.

## 📄 View Report (Recommended)

Open the fully rendered notebook:

https://nbviewer.org/github/nicolas-speranza/cse5280-building-evacuation-nicolas-speranza/blob/main/building_evacuation.ipynb

## Contents

- Mathematical formulation  
- Three-floor building geometry  
- Ramp and surface-height modeling  
- Multi-agent gradient-based simulation  
- Quantitative experiments  
- Trajectory visualizations  
- Vedo animation and video export  
- Discussion and conclusions  

## Experiments Compared

- baseline — no crowd repulsion  
- crowd_aware — includes inter-agent repulsion  
- sharp_softmin — stronger target selection  
- smooth_softmin — smoother shared attraction  

## Key Result

Structured multi-floor evacuation behavior emerges directly from optimization, with agents navigating ramps, floors, walls, and exits without explicit planning algorithms.

## Repository Files

- `building_evacuation.ipynb` — full notebook with experiments, analysis, and animation  
- `README.md` — project overview and report link  
