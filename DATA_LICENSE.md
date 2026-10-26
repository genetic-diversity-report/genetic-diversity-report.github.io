# Data licence

The tables under `data/` (and the same data embedded in `dashboard.html`) are released under
the Creative Commons Attribution-NonCommercial 4.0 International licence
(CC BY-NC 4.0, <https://creativecommons.org/licenses/by-nc/4.0/>).

Attribution: "Expósito-Alonso, M., *Genetic diversity loss by country* (genetic diversity report),
run 20261024-r3, <https://genetic-diversity-report.github.io/>".

The non-commercial condition follows from the terms of use of the upstream sources from which
the values are derived: the IUCN Red List spatial data and assessments, the Living Planet Index
database and the World Database on Protected Areas (UNEP-WCMC and IUCN) restrict commercial use
of derived products. Values derived only from openly licensed inputs (LUH2 v2h, MIT licence
attribute of the data file; Borgelt et al. 2022 plant ranges, CC0; RESOLVE Ecoregions 2017,
CC BY 4.0; Natural Earth, public domain) may be relicensed on request. The basemap
`data/countries-110m.json` is the Natural Earth 1:110m admin-0 layer (public domain) as packaged
by world-atlas 2.0.2.

Rows of the demography lens that derive from the Living Planet Database (lens `demography_lpi`)
are supplied under the Living Planet Index data terms (non-commercial use, attribution to
ZSL/WWF, onward supply under the same terms), which the Living Planet Index policy requires for
derived data; they are not relicensed under CC BY-NC 4.0. Red List categories carried per
species are unrestricted under the IUCN terms. Users who publish work based on these tables
should cite the source versions listed in README.md and the citations below.

The repository contains derived summaries only. No range polygons, no protected-area polygons
and no population time series are redistributed. The sources listed in README.md must be
credited alongside the attribution above.

## Citations and obligations

Red List: IUCN (2025). The IUCN Red List of Threatened Species. Version 2025-2.
<https://www.iucnredlist.org>. Range maps: IUCN Red List spatial data, 2022 release (mammals,
amphibians, reptiles), used in the computation and not redistributed.

Protected areas: UNEP-WCMC and IUCN (2026). Protected Planet: The World Database on Protected Areas (WDPA) and World Database on Other Effective Area-based Conservation Measures (WD-OECM), September 2026. Cambridge, UK: UNEP-WCMC and IUCN. www.protectedplanet.net — <https://www.protectedplanet.net>.

Copies of publications that use these tables are sent to IUCN (Red List terms), to UNEP-WCMC
(Protected Planet terms) and to the Living Planet Index team (Living Planet Index data terms).

LUH2 v2h: the data file's licence attribute reads MIT; the input4MIPs record of the same data
states CC BY-SA 4.0. Both are cited here; the aggregates in `data/` do not redistribute the
LUH2 grids.

Figure files under `assets/` are released under CC BY-NC 4.0, the same licence as the data,
except where a file contains only public-domain basemap material (Natural Earth), which stays
in the public domain.
