# Motorcycle-Footpeg-Bracket— Topology Optimisation

Designed and analysed a motorcycle footpeg bracket as a self-directed 
design project. Started from a solid bounding box, validated it with FEA, 
then used shape optimisation to find the minimum-material geometry.

## What I did

Modelled a 120 × 80 × 20mm bounding box in Creo with two M8 mounting 
holes and a 12mm footpeg pin hole. Calculated the load case manually 
from rider dynamics (80kg rider, combined braking + cornering = 612N), 
then ran static FEA in both Ansys Discovery and SimScale to validate.

The solid block came back with SF = 54 — massively overdesigned — which 
confirmed there was a lot of material to remove. Ran shape optimisation 
in Fusion 360 targeting 40% mass removal.

## Results

- Mass reduced from 0.507 kg to 0.308 kg (39.2% reduction)
- Max Von Mises stress: 5.10 MPa (yield = 276 MPa, SF = 54.1)
- Load case: 470N vertical + 314N braking + 235N lateral

## Tools

Creo Parametric · Ansys Discovery · SimScale · Fusion 360

## Files

- `design_space.stp` — Creo model
- `design_brief.pdf` — full documentation
- `engineering_drawing.pdf` — 2D drawing with dimensions
- `fea/` — Ansys and SimScale screenshots
- `optimisation/` — Fusion 360 topology result
