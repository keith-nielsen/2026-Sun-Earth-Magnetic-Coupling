# Data

This paper synthesizes previously published, openly available data. No bulk data
is tracked in git; the analyses pull from the public sources below.

## Data sources

| Dataset | Source | URL |
|---|---|---|
| Sunspot number (monthly, v2.0) | SILSO, Royal Observatory of Belgium | https://www.sidc.be/SILSO/ |
| Length of day (IERS EOP C04 20 v2) | IERS Earth Orientation Centre | https://www.iers.org/ |
| Solar wind / magnetospheric indices (AE, Dst, ε, V, P, IMF Bz) | NASA OMNI | https://omniweb.gsfc.nasa.gov/ |
| Effective angular momentum functions (AAM) | ESMGFZ | http://esmdata.gfz-potsdam.de/ |
| Global instrumental earthquake catalogue | ISC-GEM | http://www.isc.ac.uk/iscgem/ |
| Geomagnetic field models | ESA Swarm | https://earth.esa.int/eogateway/missions/swarm |
| Inner-core rotation estimates | Yang & Song (2023), *Nat. Geosci.* | https://doi.org/10.1038/s41561-022-01112-z |

## Reproducing the analyses

The two empirical tests (manuscript §4.6 and §4.7) draw directly from the sources
above. See [`code/README.md`](../code/README.md) for the pipeline descriptions;
the scripts are to be deposited alongside the manuscript.
