# Multimedia

## Overview

This directory houses interactive visualizations, animations, and
other supplementary media that extend the static figures in the paper.

## Planned Contents

- **Interactive 3D magnetosphere viewer** — WebGL-based visualization
  of MHD simulation output, allowing the user to rotate, zoom, and
  toggle magnetic field lines, plasma density contours, and
  magnetopause boundaries
- **Animation loops** — Time-series animations of solar wind forcing
  and magnetospheric response
- **Supplementary video** — Narrated walkthrough of key results

## Status

| Component | Status | Location |
|-----------|--------|----------|
| Static figures | Included in `paper/figures/` | `paper/figures/` |
| Interactive viewer | Planned | `multimedia/interactive/` |
| Simulation animations | Planned | `multimedia/animations/` |
| Supplementary video | Planned | `multimedia/video/` |

## Building Multimedia Assets

```bash
cd code/analysis
python render_animations.py --input ../../data/processed/ --output ../../multimedia/animations/
python build_interactive_viewer.py --output ../../multimedia/interactive/
```

## Notes

- Large rendered files (video, compiled WebGL) are stored via
  [Git LFS](https://git-lfs.com) or external hosting
- Source code for generating all multimedia is in `code/analysis/`
- See `docs/roadmap.md` for the development timeline