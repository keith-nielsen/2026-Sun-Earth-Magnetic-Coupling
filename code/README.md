# Simulation and Analysis Code

## Overview

This directory contains the code for running MHD simulations, analyzing
results, and generating figures for the paper. All code is version-controlled
alongside the manuscript to ensure full reproducibility.

## Structure

```
code/
├── experiments/          # MHD simulation run scripts
│   ├── run_mhd.py       # Main simulation driver
│   ├── config/          # Simulation parameter files
│   └── submit_jobs.sh   # HPC job submission (SLURM/PBS)
├── analysis/             # Post-processing and visualization
│   ├── generate_figures.py
│   ├── compute_metrics.py
│   └── compare_observations.py
└── requirements.txt      # Python dependencies
```

## Quick Start

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt

# Run a small test simulation
cd experiments
python run_mhd.py --config config/default.yaml --output ../../data/processed/

# Generate figures from pre-computed results
cd ../analysis
python generate_figures.py --input ../../data/processed/ --output ../../paper/figures/
```

## Dependencies

See `requirements.txt` for pinned versions. Key packages:

- `numpy`, `scipy` — numerical computation
- `matplotlib` — publication-quality figures
- `h5py` / `netCDF4` — simulation output I/O
- `astropy` — coordinate transformations and units

## Notes

- All simulations should be run from this directory
- Figure output goes to `paper/figures/` for inclusion in the manuscript
- See `experiments/config/` for the exact parameter sets used in the paper