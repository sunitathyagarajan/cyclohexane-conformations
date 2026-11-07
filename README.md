# Cyclohexane Conformations

An interactive learning module for organic chemistry students on the conformations of cyclohexane.

**Live site:** https://sunitathyagarajan.github.io/cyclohexane-conformations/

## What's in the module

1. **Why isn't cyclohexane flat?** Angle and torsional strain in a planar ring, with ring-strain data for C3–C6 cycloalkanes.
2. **The chair and the boat.** Two rotatable 3D models that turn together, with axial/equatorial and flagpole hydrogens highlighted and a Newman view down C2–C3.
3. **The ring flip.** An animated chair → half-chair → twist-boat → boat → twist-boat → half-chair → chair pathway, synced to an energy diagram drawn to scale. An optional methyl group shows the 1,3-diaxial interaction appearing after the flip.
4. **Thermodynamics.** Energies of each conformation, ΔG° = −RT ln K, A-values with a 3D 1,3-diaxial strain explorer for nine substituents, a conformer population calculator, and the Eyring ring-flip rate with its NMR consequences.
5. **Check your understanding.** Five multiple-choice questions with explanations and a score.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole module: one self-contained page (HTML, CSS and JavaScript). |
| `cyclohexane-module.html` | Redirects old links to `index.html`. |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are, without Jekyll processing. |

The page loads two things from the web: [three.js r128](https://threejs.org/) from cdnjs for the 3D models, and the Open Sans font from Google Fonts (used where Segoe UI is not installed). Everything else is inline, so there is no build step.

## Publishing on GitHub Pages

1. Push this repository to GitHub.
2. On GitHub, open **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**, then pick the **main** branch and the **/ (root)** folder, and click **Save**.
4. After a minute or two the site appears at the live-site address above.

## Running it locally

Open `index.html` in any modern browser. The 3D models need WebGL and an internet connection (to load three.js).

## Notes on the data

Energies are the rounded literature values most organic chemistry textbooks use (chair 0, twist-boat 5.5, boat 6.9, half-chair 10.8 kcal/mol). The 3D geometries are generated from Cremer–Pople ring-puckering coordinates with ideal bond lengths, so distances measured in the models are close to, but not exactly, experimental values.
