# Source discrepancies found during integration

While integrating the manuscript and building a verified `paper/references.bib`,
every DOI in the source was checked against `doi.org` and Crossref. Three issues
surfaced that originate in the source manuscript and need an author decision.
The manuscript body (`paper/manuscript.md`) was **left verbatim**; only the
machine-readable `references.bib` was corrected to the true published records.

## 1. McIntosh references swapped / mislabeled (needs in-text fix)

The two McIntosh entries had their DOIs swapped, with wrong years and volumes:

| Manuscript says | Actual (verified via Crossref) |
|---|---|
| McIntosh et al. **2019**, "Overlapping magnetic activity cycles…", *Sol. Phys.* **294**, 88, doi `…s11207-019-1474-y` | This title is **McIntosh et al. 2020**, *Sol. Phys.* **295**, 163, doi **`10.1007/s11207-020-01723-y`** |
| McIntosh et al. **2021**, "What the sudden death of solar cycles…", *Sol. Phys.* **296**, 189, doi `…s11207-021-01929-y` (does **not** resolve) | This title is **McIntosh et al. 2019**, *Sol. Phys.* **294**, 88, doi **`10.1007/s11207-019-1474-y`** |

The DOI `10.1007/s11207-019-1474-y` actually belongs to the *"sudden death"* paper
(2019), and `10.1007/s11207-021-01929-y` is not a registered DOI.

**`references.bib` now uses the correct records** (keys `mcintosh2019` = "sudden
death" 2019; `mcintosh2020` = "overlapping cycles" 2020).

**Resolved in the manuscript.** The in-text citations and the References list have
been corrected, attributing each claim to the paper that actually supports it:

- **Terminator** definition and the **step-function rise in solar/geomagnetic
  activity** at terminators → McIntosh et al. **2019** (*Sol. Phys.* 294:88, the
  "sudden death"/solar-interior paper). This covers the three in-text uses in
  §4.2 (inner-core oscillation), §6.1 (Prediction 1), and the glossary, plus the
  terminator clause in §4.3 — all of which already read "2019" and now resolve to
  the correct record.
- **Solar Cycle 25 stronger than the consensus forecast** (§4.3) → McIntosh et al.
  **2020** (*Sol. Phys.* 295:163, the "overlapping cycles" paper, whose result is
  precisely a stronger-than-consensus SC25 forecast). The §4.3 sentence that read
  "(McIntosh et al., 2021)" — a year with no matching publication — was the only
  wrong in-text year; it is now split so the terminator claim cites 2019 and the
  forecast claim cites 2020.

> Please sanity-check the §4.3 attribution: the added `(McIntosh et al., 2020)`
> on the forecast sentence is editorial and easy to drop if you prefer.

## 2. Nayar et al. 2002 DOI does not resolve

`10.5194/angeo-20-1061-2002` returns 404. *Annales Geophysicae* volume 20 (2002)
predates Copernicus's DOI registration for the journal, so this article most likely
has no registered DOI. The `references.bib` entry keeps full bibliographic details
but omits the DOI.

**Action for author:** confirm whether a registered DOI exists; if not, cite by
volume/pages (and optionally a stable publisher URL).

## 3. Duplicate reference entry (cosmetic)

"Knudsen et al. 2008, *Earth Planet. Sci. Lett.* **272**, 319–329" appears **twice**
in the manuscript's References section. `references.bib` contains a single entry
(`knudsen2008`).

**Action for author:** remove the duplicate paragraph from the manuscript's
References list.
