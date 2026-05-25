# Solar Magnetic Forcing of Earth's Magnetosphere: Magnetohydrodynamic Modeling

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Last Commit](https://img.shields.io/github/last-commit/keith-nielsen/2026-Magnetics-Solar-Forcing-Earth-Magnetohydrodynamics)](https://github.com/keith-nielsen/2026-Magnetics-Solar-Forcing-Earth-Magnetohydrodynamics)
[![Paper Compilation](https://github.com/keith-nielsen/2026-Magnetics-Solar-Forcing-Everything/actions/workflows/paper.yml/badge.svg)](.github/workflows/paper.yml)

> **Originated:** 2026 · **Latest release:** [v1.0](https://github.com/keith-nielsen/2026-Magnetics-Solar-Forcing-Earth-Magnetohydrodynamics/releases/tag/v1.0)

## Overview

This repository contains the full reproducible research package for a magnetohydrodynamic (MHD) study of solar magnetic forcing on Earth's magnetosphere. The work reproduces and extends established results in solar-terrestrial physics, examining how variations in the interplanetary magnetic field (IMF) and solar wind parameters modulate magnetospheric dynamics.

**Keywords:** `magnetohydrodynamics` `solar-terrestrial-physics` `magnetosphere` `solar-wind` `magnetic-reconnection` `space-weather`

## Repository Structure

```
├── paper/             # Manuscript source (LaTeX), figures, bibliography
│   ├── manuscript.tex
│   ├── references.bib
│   └── figures/
├── code/              # Reproducible analysis and simulation code
│   ├── experiments/   # MHD simulation run scripts
│   ├── analysis/      # Post-processing and visualization
│   └── requirements.txt
├── data/              # Example datasets and data provenance
├── models/            # Saved model configurations (weights hosted externally)
├── multimedia/        # Interactive visualizations, animations, auxiliary media
├── docs/              # Roadmap, replication guide, supplementary notes
└── .github/workflows/ # CI: automated paper compilation
```

## Reproducibility

All results in this paper can be reproduced from this repository:

```bash
# 1. Set up the environment
cd code
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt

# 2. Run simulations
cd experiments
python run_mhd_simulations.py

# 3. Generate figures
cd ../analysis
python generate_figures.py

# 4. Build the paper
cd ../../paper
make
```

See [`docs/replication.md`](docs/replication.md) for a detailed step-by-step guide.

## Citation

If you use this work in your research, please cite:

```bibtex
@article{nielsen2026solar,
  author  = {Nielsen, Keith},
  title   = {Solar Magnetic Forcing of Earth's Magnetosphere: 
             Magnetohydrodynamic Modeling and Analysis},
  journal = {TODO — Journal Name},
  year    = {2026},
  doi     = {TODO — DOI}
}
```

See [`CITATION.cff`](CITATION.cff) for machine-readable citation metadata.

## License

This project is licensed under the MIT License — see the [`LICENSE`](LICENSE) file for details.

## Roadmap

- [x] Initial manuscript and simulation framework (v1.0)
- [ ] Interactive 3D magnetosphere visualization
- [ ] Expanded parameter sweeps for IMF orientation
- [ ] Data-driven validation against satellite observations
- [ ] Real-time space weather prediction interface

See [`docs/roadmap.md`](docs/roadmap.md) for the full development plan.