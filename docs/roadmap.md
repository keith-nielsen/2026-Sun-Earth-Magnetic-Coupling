# Development Roadmap

> **Last updated:** 2026

This document outlines the planned development trajectory for this
project beyond the initial manuscript release.

## Phase 1: Paper Publication (v1.0) ✅

- [x] Manuscript draft (LaTeX, revtex4-2)
- [x] Core MHD simulation framework
- [x] Reproduction of key literature results
- [x] GitHub repository with CI-compiled paper
- [x] MIT License and CITATION.cff

## Phase 2: Interactive and Extended Materials

- [ ] **Interactive 3D visualization** — WebGL-based magnetosphere
      viewer using simulation output
  - Framework candidate: Three.js / VTK.js
- [ ] **Extended parameter sweeps** — Systematic exploration of IMF
      clock angle, solar wind velocity, and number density
- [ ] **Comparison with in-situ observations** — THEMIS, MMS, and
      Cluster satellite data for model validation
- [ ] **Animation gallery** — Time-lapse videos of simulated
      magnetospheric dynamics under different solar wind conditions

## Phase 3: Operational Tools

- [ ] **Real-time space weather prediction interface** — Lightweight
      web app that accepts solar wind input and predicts
      magnetospheric response
- [ ] **API endpoint** — REST API for programmatic access to
      simulation results
- [ ] **Containerized deployment** — Docker/Singularity images for
      reproducible execution

## Phase 4: Community and Documentation

- [ ] **Jupyter notebook tutorials** — Guided walkthroughs for
      reproducing figures
- [ ] **Zenodo archiving** — DOI assignment for the repository
- [ ] **Supplementary data release** — Simulation output on
      Zenodo/HuggingFace Datasets
- [ ] **Video abstract** — Short narrated overview of the paper

## Contributing

Interested in contributing? See open issues for tasks tagged
`good-first-issue` or `help-wanted`.

---

**Legend:** ✅ Complete | 🔄 In progress | ⬜ Not started