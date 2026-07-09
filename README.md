# EPYK Soft Finger Lab

Interactive simulator of the bending pneumatic artificial muscle (EPYK) — the 6-chamber
silicone finger from Project 122M619 — showing the effect of supply pressure, wall
thickness (2 / 3 / 4 mm) and silicone material on bending angle, fingertip force and
bending moment. All curves are driven by the experimental tables (3.6–3.8) and Ansys
FEA results (Table 3.2) of the project final report.

## Deploy to GitHub Pages

1. Create a repository (e.g. `epyk-soft-finger-lab`) and push these five files to its root:
   `index.html`, `manifest.json`, `sw.js`, `icon-192.png`, `icon-512.png`.
2. Repository → Settings → Pages → Source: **Deploy from a branch**, Branch: `main`, folder `/ (root)`.
3. Open `https://<username>.github.io/epyk-soft-finger-lab/` — the app is installable
   (Add to Home Screen) and works offline after the first visit.

All paths are relative, so it works from any repo subpath without changes.

## Data provenance

- Bending angle vs pressure: report Tables 3.6 (experiment) and 3.2 (FEA, Yeoh 2nd-order).
- Fingertip force: Tables 3.7 (blocked, 0°) and 3.8 (maximum, gauge normal to tip).
- Burst pressures: 110 / 130 / 140 kPa for t = 2 / 3 / 4 mm (VRM-520).
- Material properties: Tables 3.1, 3.3; VRM-520 stress–strain: Table 3.5.
- Finger tests were performed on VRM-520 only; other materials are shown via
  Shore-hardness (Gent) stiffness scaling and are marked "Estimated" in the UI.
