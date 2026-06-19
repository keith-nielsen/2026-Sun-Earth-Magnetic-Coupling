# Development TODO

> Outstanding work for the manuscript and supporting materials.
> See [docs/roadmap.md](docs/roadmap.md) for the longer-term plan.

**Status:** Preprint draft integrated; supporting materials in progress.

## Immediate

- [ ] Resolve the reference issues in [docs/source-discrepancies.md](docs/source-discrepancies.md)
      (McIntosh citation years/DOIs, Nayar 2002 DOI, duplicate Knudsen entry).
- [ ] Fill manuscript front matter: corresponding-author email, Acknowledgments, Funding.
- [ ] Deposit the analysis pipelines for the two empirical tests (§4.6, §4.7) under `code/`.
- [ ] Deposit Supplements A–F and interactive models S1–S9 referenced in the text.

## Short-term

- [ ] Choose a target journal and generate the journal-specific LaTeX from `make tex`.
- [ ] Polish PDF typography: a few Unicode glyphs (Greek, super/subscripts, ≈)
      don't render in the default PDF font. HTML renders them fine. Fix with a
      Unicode-aware font or a `newunicodechar` preamble when convenient.
- [ ] Add ORCID to `CITATION.cff`.
- [ ] (Optional) Phase B citations: convert in-text citations to Pandoc `[@key]`
      form and enable `--citeproc` for auto-generated, journal-styled references.

## Medium-term

- [ ] Assign a Zenodo (or other) DOI on first release.
- [ ] Consider renaming the repository — the current name still references
      "Magnetohydrodynamics" / "Magnetosphere" from the earlier scaffolding,
      whereas the paper is about coupling into Earth's interior.

---

*Last updated: 2026-06-19*
