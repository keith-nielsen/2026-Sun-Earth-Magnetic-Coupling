# Data Directory

## Policy

This directory contains the data used in this study. Due to size constraints,
only small example or synthetic datasets are tracked in git. Full datasets
are archived separately.

## Contents

- `raw/` — Original data as obtained from sources (e.g., OMNI database exports).
  Not version-controlled; see `sources.md` for download instructions.
- `processed/` — Cleaned, normalized, or derived datasets used in the paper's
  figures and analysis.

## Data Sources

| Dataset | Source | URL | Citation |
|---------|--------|-----|----------|
| OMNI solar wind data | NASA OMNIWeb | https://omniweb.gsfc.nasa.gov | King & Papitashvili (2005) |
| [TODO — additional sources] | | | |

## Reproducing the Data

Run the following to download and process all datasets:

```bash
cd code/analysis
python download_data.py --output ../../data/raw/
python preprocess_data.py --input ../../data/raw/ --output ../../data/processed/
```

## Large Data

Full simulation output and large observational datasets are archived at:

- **Zenodo:** [TODO — DOI]
- **Size:** ~XX GB

To reproduce results without downloading the full archive, see `docs/replication.md`.