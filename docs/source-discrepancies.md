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

**Action for author:** update the in-text citation years and the manuscript's own
References list — the "overlapping cycles" work should be cited as **2020** and the
"sudden death" work as **2019**. Check each in-text use of `McIntosh (2019)` /
`McIntosh (2021)` to confirm it points at the intended paper.

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
