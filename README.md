# Truss Simulator v2

**Live demo: https://3uripides.github.io/truss-simulator-v2/**

![Screenshot](<img width="1205" height="857" alt="image" src="https://github.com/user-attachments/assets/c9a54c78-b6d2-415c-9858-2212e21300aa" />
)

A browser-based truss simulator with a **balsa wood strength check** added. It is a personal recreation, built for learning, of the [Truss Simulator from JHU Engineering Innovation](https://ei.jhu.edu/truss-simulator/). It is not affiliated with or endorsed by Johns Hopkins University, and the original is the authoritative tool.

## Features

- Design trusses: add, delete and move nodes, members, forces and supports (pin, horizontal roller, vertical roller).
- Click and drag nodes and force arrows directly in the Design tab (snaps to the grid).
- Solves member forces live with the method of joints; tension is blue, compression is red, reactions are green. A matrix view is available in the Solve tab.
- Display & Dimensions: units, workspace size, snap grid, zoom/pan, label toggles.
- Import & Export: pre-built trusses and save/load as a file.
- **Balsa Wood tab (new):** enter stick size, density, modulus, tensile and compressive strength, buckling factor and a strength factor for glue joints. It finds each member's limit (tension break, crushing or Euler buckling), the weakest member, and the estimated failure load in N and grams.

## Limits of the balsa model

Pin-jointed truss, axial forces only. Bending, glue-joint shear and stick defects are not modeled, so the failure load is an upper bound. Test your real bridge. Pre-built trusses 2-4 are my own examples, not copies of the original's.

## Run locally

Open `index.html` in a browser. No build step or dependencies.
