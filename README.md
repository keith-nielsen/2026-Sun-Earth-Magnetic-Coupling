# Sun-Earth Magnetic Coupling: A Unified Energy Framework for Solar Forcing of the Earth's Interior

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Last Commit](https://img.shields.io/github/last-commit/keith-nielsen/2026-Sun-Earth-Magnetic-Coupling)](https://github.com/keith-nielsen/2026-Sun-Earth-Magnetic-Coupling)
[![Paper Compilation](https://github.com/keith-nielsen/2026-Sun-Earth-Magnetic-Coupling/actions/workflows/paper.yml/badge.svg)](.github/workflows/paper.yml)

> **Author:** Keith Nielsen (independent researcher) · **Status:** Preprint in
> preparation for submission to a peer-reviewed journal.

## Overview

This repository holds the manuscript and supporting materials for a
cross-disciplinary **synthesis paper** proposing that a fraction of solar
magnetic energy couples into Earth's liquid outer core through geomagnetic
field lines, supplementing internal heat sources and influencing core dynamics.

It is **not** a numerical MHD-simulation study. The paper synthesizes published
observational data and theoretical constraints from heliophysics, magnetospheric
physics, geodynamics, and seismology, and reports **two empirical tests on public
data**:

1. A direct test of a predicted phase correlation between the solar
   quasi-sexennial oscillation (QSO) and the 5.9-year length-of-day (LOD)
   oscillation — which returns a **null result**, reported plainly.
2. A test of LOD residuals against magnetospheric energy input (NASA OMNI
   proxies), with the atmospheric contribution removed — a **suggestive,
   Hale-cycle-modulated** signal.

The framework yields fifteen testable predictions, including five forward
predictions with specific time windows.

**Keywords:** `solar-terrestrial-coupling` `geodynamo` `magnetosphere`
`core-mantle-boundary` `earth-energy-budget` `inner-core-oscillation`
`space-climate`

## Repository Structure

```
├── paper/                    # Manuscript (canonical source) + bibliography
│   ├── manuscript.md         # The paper, in Markdown (source of truth)
│   ├── references.bib        # Machine-readable references (DOIs verified)
│   ├── Makefile              # Pandoc build: PDF / HTML / LaTeX export
│   └── figures/              # Figures (none embedded in the current draft)
├── code/                     # Analysis pipelines for the two empirical tests
├── data/                     # Public data sources & provenance (no bulk data)
├── docs/                     # Roadmap, replication guide, source-discrepancies
├── models/                   # (reserved)
├── multimedia/               # Interactive supplementary models S1–S9 (planned)
└── .github/workflows/        # CI: builds the paper PDF/HTML on push
```

## Building the paper

The manuscript is Markdown; the PDF is produced with [Pandoc](https://pandoc.org)
and [Tectonic](https://tectonic-typesetting.github.io):

```bash
cd paper
make           # -> manuscript.pdf  (Pandoc + Tectonic)
make html      # -> manuscript.html (no LaTeX toolchain needed)
make tex       # -> manuscript.tex  (starting point for a journal template)
```

You can also just read [`paper/manuscript.md`](paper/manuscript.md) directly on
GitHub.

## Data availability

The paper synthesizes previously published, openly available data. See
[`data/README.md`](data/README.md) for the full list. Primary sources:

- Sunspot numbers — SILSO v2.0, Royal Observatory of Belgium
- Length-of-day — IERS Earth Orientation Parameters (EOP C04)
- Solar wind / magnetospheric indices — NASA OMNI
- Atmospheric angular momentum — ESMGFZ effective angular momentum functions
- Earthquake catalog — ISC-GEM Global Instrumental Earthquake Catalogue
- Geomagnetic field models — ESA Swarm

## Citation

This is a preprint; citation metadata is provisional. See
[`CITATION.cff`](CITATION.cff). A DOI will be assigned on release.

## License

MIT — see [`LICENSE`](LICENSE).

## Notes for collaborators

- [`docs/source-discrepancies.md`](docs/source-discrepancies.md) records
  reference-metadata issues found in the current draft that need an author
  decision (two DOI corrections and a duplicate entry).
- [`TODO.md`](TODO.md) lists outstanding work; [`docs/roadmap.md`](docs/roadmap.md)
  the longer-term plan.
