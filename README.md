# Truss Simulator v2

**Live demo: https://3uripides.github.io/truss-simulator-v2/**

<img width="1205" height="857" alt="Truss Simulator v2 screenshot" src="https://github.com/user-attachments/assets/c9a54c78-b6d2-415c-9858-2212e21300aa" />

A browser-based truss simulator with a **balsa wood strength check** added. It is a personal recreation, built for learning, of the [Truss Simulator from JHU Engineering Innovation](https://ei.jhu.edu/truss-simulator/). It is not affiliated with or endorsed by Johns Hopkins University, and the original is the authoritative tool.

## Features

- **Design:** add nodes, members, forces and supports (pin, horizontal roller, vertical roller). Members, forces and supports can start on blank space (a node is created there).
- **Move and select:** drag nodes and force arrows, box-select several nodes and drag them together, Shift+click to add to the selection, Delete to remove.
- **Delete:** single node/member/force, forces only, a support only, or everything.
- **Undo / redo:** Ctrl+Z and Ctrl+Y (also buttons in the Design row).
- **Double stacking:** make any member two sticks side by side (shown bold, e.g. 3 x 3 mm becomes 3 x 6 mm).
- Solves member forces live with the method of joints; tension is blue, compression is red, reactions are green. A matrix view is in the Solve tab. A **Color view** button switches to a green-to-red stress view (how close each member is to failing).
- **Balsa Wood tab:** stick size, density, modulus, tensile and compressive strength, buckling factor and a glue/defect strength factor. Finds each member's limit (tension break, crushing or Euler buckling), the weakest member, and the estimated failure load in N and grams.
  - **Test load slider:** scale the applied load and watch the result update.
  - **Animate load test:** ramps the load until the first member breaks.
  - **Where to put the load:** failure load for a single weight at each node.
  - **Parts list:** cut list of stick lengths, counts, total length and weight.
- **Import & Export:** pre-built trusses, Download bridge (.json), Upload bridge, and Export image (.png).
- **Autosave** in the browser, dark mode, and a **Guide** dropdown (top right) that explains every feature.
- Display & Dimensions: units, window size, snap grid, zoom/pan, label toggles.

## Limits of the balsa model

Pin-jointed truss, axial forces only. Bending, glue-joint shear and stick defects are not modeled, so the failure load is an upper bound. Test your real bridge. Pre-built trusses 2-4 are my own examples, not copies of the original's.

## Run locally

Open `index.html` in a browser. No build step or dependencies.
