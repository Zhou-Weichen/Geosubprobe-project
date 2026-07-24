# Geosubprobe — Project Page

Self-contained academic project page for
**Understanding Geometric Representations in Self-Supervised Vision Transformers via Subspace Intervention** (ECCV 2026).

Everything is inlined into `index.html` (CSS + JS, no build step, no external CDNs).
It works by just double-clicking `index.html` locally, and it is portable — this whole
folder can be dropped into any repo root unchanged.

```
project_page/
├── index.html            # the entire page (self-contained)
└── assets/
    ├── framework.png      # method / teaser figure (already included)
    ├── fig2_recovery.png  # ← drop your exported figures here (optional, placeholders shown until then)
    ├── fig3_qualitative.png
    ├── fig4_energy.png
    ├── fig5_layerwise.png
    ├── fig6_affinity.png
    ├── fig7_normalized.png
    └── fig8_stability.png
```

## Add the real figures

The page shows a labeled placeholder for each of Figs 2–8. To fill one in, export the
figure as a PNG (or SVG) and save it in `assets/` under the **exact filename** listed
above — it appears automatically, no HTML edits needed. Filenames the page expects:

| File | Paper figure |
|------|--------------|
| `assets/fig2_recovery.png`    | Fig. 2 — Absolute recovery / recovery efficiency |
| `assets/fig3_qualitative.png` | Fig. 3 — Qualitative subspace interventions (depth grid) |
| `assets/fig4_energy.png`      | Fig. 4 — Energy distribution across singular directions |
| `assets/fig5_layerwise.png`   | Fig. 5 — Layer-wise subspace analysis |
| `assets/fig6_affinity.png`    | Fig. 6 — Qualitative task affinity in DINOv2 |
| `assets/fig7_normalized.png`  | Fig. 7 — Normalized probing performance |
| `assets/fig8_stability.png`   | Fig. 8 — Subspace stability |

You may also replace `assets/framework.png` with a higher-resolution export.

## Publish as a standalone project site (like `username.github.io/project/`)

1. Create a new empty GitHub repo, e.g. `Geosubprobe-project`.
2. Copy the **contents of this folder** (`index.html` + `assets/`) into the repo root and push:
   ```bash
   git init
   git add .
   git commit -m "Add project page"
   git branch -M main
   git remote add origin https://github.com/<user>/Geosubprobe-project.git
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Source: `main` branch, `/ (root)` → Save**.
4. The page goes live at `https://<user>.github.io/Geosubprobe-project/` after a minute.
