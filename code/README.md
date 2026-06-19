# Analysis code

This directory is for the analysis pipelines behind the paper's two empirical
tests. The paper is a synthesis/framework study — there is **no MHD simulation
code** (the earlier scaffolding here described simulations that were never part
of this work and has been removed).

> **Status:** pipelines to be deposited. The methodology is fully specified in
> the manuscript (§4.6, §4.7) and Supplements E and F. The scripts that produced
> the reported numbers should be added here so the results are reproducible.

## Pipeline 1 — QSO–LOD phase correlation (§4.6, Supplement E)

Tests the predicted phase correlation between the solar quasi-sexennial
oscillation and the 5.9-year length-of-day oscillation. **Result: null.**

- Inputs: monthly sunspot number (SILSO v2.0), daily LOD (IERS EOP C04 20 v2),
  1962–2025.
- Method: detrend; 5.0–7.0 yr band-pass (4th-order Butterworth, zero-phase
  `scipy.signal.filtfilt`); zero-lag correlation and lag structure; Hilbert
  instantaneous-phase / phase-locking value; significance vs phase-randomized
  Fourier surrogates and AR(1) red-noise surrogates; band-edge sensitivity
  sweep; synthetic positive/negative controls.

## Pipeline 2 — LOD residual vs magnetospheric energy input (§4.7, Supplement F)

Tests whether rotation anomalies track magnetospheric energy input.

- Inputs: monthly LOD residuals; six NASA OMNI proxies (AE, Dst, Akasofu
  epsilon, solar-wind speed, dynamic pressure, IMF Bz), 1963–2025; ESMGFZ
  effective angular momentum functions (AAM), 1976–2025.
- Method: broadband and lagged correlations; subtraction of the atmospheric
  angular momentum contribution; 5-year running correlation vs the epsilon
  function; pre/post-2020 shift analysis.

## Environment

See [`requirements.txt`](requirements.txt). Core dependencies: `numpy`, `scipy`,
`pandas`, `matplotlib`.
