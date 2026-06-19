# Replication guide

This is a synthesis paper with two empirical tests on public data. There are no
large simulations to run; reproduction means rebuilding the document and (once
the analysis scripts are deposited) re-running the two tests.

## Build the paper

```bash
git clone https://github.com/keith-nielsen/2026-Sun-Earth-Magnetic-Coupling.git
cd 2026-Sun-Earth-Magnetic-Coupling/paper
make          # manuscript.pdf  (requires pandoc + tectonic)
make html     # manuscript.html (requires only pandoc)
```

Install [Pandoc](https://pandoc.org/installing.html) and
[Tectonic](https://tectonic-typesetting.github.io/) (the latter only for PDF).
CI builds both on every push — see `.github/workflows/paper.yml`.

## Reproduce the empirical analyses

The analysis pipelines are described in [`code/README.md`](../code/README.md)
(§4.6 QSO–LOD phase correlation; §4.7 LOD residual vs magnetospheric input) and
will be deposited under `code/`. Data sources are listed in
[`data/README.md`](../data/README.md). With the scripts present:

```bash
cd code
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
# then run the pipeline scripts (see code/README.md)
```

All inputs are public (SILSO, IERS, NASA OMNI, ESMGFZ, ISC-GEM, ESA Swarm), so
the analyses can be reproduced independently from the cited datasets.
