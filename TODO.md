# Solar Magnetic Forcing — Development TODO

> Near-term work items for the MHD modeling paper and simulation framework.
> See [docs/roadmap.md](docs/roadmap.md) for the broader vision.

**Status:** Skeleton — paper content and simulation code need writing

## Immediate

- [ ] Write manuscript — fill in Results, Discussion, and Conclusion sections of `paper/manuscript.tex`
- [ ] Develop MHD simulation code — implement `code/experiments/run_mhd.py` and analysis pipeline in `code/analysis/`
- [ ] Generate publication-quality figures from simulation output → `paper/figures/`
- [ ] Validate references — confirm all citations in `references.bib` are correct and complete

## Short-term

- [ ] Interactive 3D magnetosphere viewer — WebGL visualization (per roadmap Phase 2)
- [ ] Compare model results against OMBI satellite observations for validation
- [ ] Assign Zenodo DOI to the repository once the paper is in shape
- [ ] Add ORCID to CITATION.cff and author metadata

## Medium-term

- [ ] Interactive visualization gallery — time-lapse animations of simulated magnetospheric dynamics
- [ ] Containerized reproduction — Docker image for running simulations without manual setup
- [ ] Jupyter notebook tutorials — guided walkthroughs for reproducing figures

---

*Items move to GitHub Issues when concrete enough to assign. Last updated: 2026-05-26*