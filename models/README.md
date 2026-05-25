# Models

## Overview

This directory stores model configurations, checkpoints, and metadata
for the MHD simulations. Due to file size limitations, large model
weights and simulation snapshots are **not** tracked in git.

## Contents

| File | Description | Git-tracked? |
|------|-------------|-------------|
| `config.yaml` | Default simulation parameters | Yes |
| `mesh/` | Grid configuration files | Yes |
| `*.h5` / `*.nc` | Large simulation outputs | No |

## Where to Find Large Files

Full simulation snapshots and trained model weights are archived:

- **Zenodo:** [TODO — DOI]
- **HuggingFace:** [TODO — HF dataset link]
- **Single-file download:** Available on request

## Reproducing Models

All models can be regenerated from scratch:

```bash
cd code/experiments
python run_mhd.py --config ../../models/config.yaml --output ../../data/processed/
```

See `docs/replication.md` for the full procedure.