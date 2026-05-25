# Replication Guide

## Purpose

This document provides a step-by-step guide to reproduce all results
in the paper. A reviewer or interested researcher should be able to
follow these instructions and obtain identical results.

## Prerequisites

- **Hardware:** Minimum 8 GB RAM, 4 CPU cores (16+ GB RAM recommended
  for full simulation runs)
- **Software:** Python 3.10+, LaTeX distribution (TeX Live 2023+),
  git
- **Disk:** ~50 GB for full simulation output (or use pre-computed
  data from Zenodo)

## Step 1: Clone the Repository

```bash
git clone https://github.com/keith-nielsen/2026-Magnetics-Solar-Forcing-Earth-Magnetohydrodynamics.git
cd 2026-Magnetics-Solar-Forcing-Earth-Magnetohydrodynamics
```

## Step 2: Set Up the Python Environment

```bash
cd code
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Step 3: Obtain the Data

**Option A: Download pre-computed data (fast, ~2 GB)**

```bash
# Download from Zenodo
cd data
wget https://zenodo.org/records/TODO/mhd-simulation-output.tar.gz
tar xzf mhd-simulation-output.tar.gz
```

**Option B: Generate from raw data (slow, requires HPC access)**

```bash
# Download raw OMNI data
cd code/analysis
python download_data.py

# Run simulations
cd ../experiments
python run_mhd.py --config config/default.yaml --output ../../data/processed/
python run_mhd.py --config config/northward-imf.yaml --output ../../data/processed/
python run_mhd.py --config config/southward-imf.yaml --output ../../data/processed/
```

## Step 4: Generate Figures

```bash
cd code/analysis
python generate_figures.py --input ../../data/processed/ --output ../../paper/figures/
```

## Step 5: Build the Paper

```bash
cd paper
make
```

The output PDF will be at `paper/manuscript.pdf`.

## Expected Output

After following the steps above, you should have:

- `paper/manuscript.pdf` — the compiled paper
- `paper/figures/` — all figures used in the paper
- `data/processed/` — the processed simulation data
- Reproducible environment via `code/requirements.txt`

## Verification

To verify your reproduction matches the published results:

```bash
cd code/analysis
python verify_reproduction.py --reference ../../data/reference/ --generated ../../data/processed/
```

This script checks key quantitative metrics (dayside reconnection
rate, magnetopause stand-off distance, cross-polar-cap potential)
against the published values.

## Troubleshooting

| Problem | Likely Cause | Solution |
|---------|-------------|----------|
| `lualatex: command not found` | Missing LaTeX | Install TeX Live: `sudo apt install texlive-latex-extra` |
| Simulation crashes | Insufficient memory | Reduce grid resolution in `config.yaml`, or use pre-computed data |
| Figures don't match | Version mismatch | Run `pip install -r requirements.txt --upgrade` |

## Containerized Reproduction (Alternative)

A Docker image with all dependencies pre-installed is available:

```bash
docker pull ghcr.io/keith-nielsen/mhd-solar-forcing:latest
docker run --rm -v $(pwd):/workspace ghcr.io/keith-nielsen/mhd-solar-forcing \
  bash -c "cd /workspace && make -C paper"
```