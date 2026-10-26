# Genetic diversity loss by country

A report by Moisés Expósito-Alonso (University of California Berkeley; Innovative Genomics
Institute; Howard Hughes Medical Institute): a model-based estimate, for every country, of how much genetic diversity the mapped
plants, mammals, amphibians and reptiles have lost since 1850 as their primary habitat
was converted. Live page: <https://genetic-diversity-report.github.io/>
(an independent research product; not a CBD document).

Every value is a model-based estimate. It is modelled from global datasets, not national data, and has not been validated by any Party.
It is not the headline indicator A.4 and is not a substitute for it; it is intended to be
read alongside it and the complementary indicator on populations maintained.
Country values are not an ordering of countries: species coverage, priors and range data
differ by country, so a value is read with its species count and confidence, never as a rank.

## Current run

<!-- run:begin -->
| | |
|---|---|
| run id | 20261024-r3 |
| methods version | 0.1.2 |
| built (UTC) | 2026-10-26 |
| countries in scope | 210 (every country with LUH2 land) |
| species | 49,287 plants, mammals, amphibians and reptiles with a range map reaching the 210 countries; 48,064 enter the run's loss table, in 186,218 species × country pairs (the bundle carries the default-key subsets of that table) |
| estimates at the default keys | 169 countries on primary habitat, 27 more under the natural-habitat definition, 14 without an area estimate |
<!-- run:end -->

Birds are not included. The land-use record ends in 2015. The interval around each value
covers exponent uncertainty and species sampling only.

## What is in this repository

| path | content |
|---|---|
| `index.html` | the page (static; loads `data/` by relative path, routes with URL hashes) |
| `methods_panel.md` | the methods and provenance text shown inside the page |
| `data/bundle_manifest.json` | every file of the bundle with its size and hash, the run id, the scope, the provenance-id rule, the source tables |
| `data/country_summary_default.json` | the default-key values for all countries (home map, search, compare) |
| `data/country/<ISO3>.json` | one compact file per country: area and protection lenses by biome and taxon, 1850 and 1970 baselines |
| `data/country_summary/<ISO3>/`, `data/species/<ISO3>/` | full tables, including per-species rows, for Armenia, Spain, Brazil, Kenya, the United States and the pooled unit |
| `data/country_protection_area.json` | protected-area shares per country and biome, from the public WDPA and WD-OECM |
| `dashboard.html` | a single-file offline copy of the page with the same data (38 MB) |

Numbers are produced by the author's pipeline (`cop17-2026/`, to be published separately); this
repository holds the built page and its data only. Each run is one
commit, so earlier runs stay in the history. An archived copy of the full result tables
with a DOI is planned.

## Verifying a number

Every displayed value carries a provenance id. `bundle_manifest.json` gives the rule by
which the id is formed from the run id, the table and the keys, so a value on the page can
be traced to its row in `data/` and to the estimator described in `methods_panel.md`.

## Sources

LUH2 v2h land-use reconstruction (850–2015) · Natural Earth admin-0 v5.1.1 · RESOLVE
Ecoregions 2017 · WDPA and WD-OECM (September 2026 release; public polygons only, none
redistributed) · IUCN Red List assessments 2025-2 and IUCN spatial data 2022-1 (mammals,
amphibians, reptiles; range maps are used in the computation and not redistributed) ·
Borgelt et al. 2022 plant ranges · Living Planet Index 2024 (derived summaries only) ·
diversity–area exponents from Schmidt et al. 2026, Mualim et al. 2026, RepAdapt and
Expósito-Alonso et al. 2022 · Mastretta-Yanes et al. 2024 pilot.

## Terms

Page code (`index.html`, the page part of `dashboard.html`) and the build scripts kept in the
working group's project folder: MIT (see `LICENSE`). Data tables under `data/`, the data embedded
in `dashboard.html` and the text of `methods_panel.md`: CC BY-NC 4.0 (see `DATA_LICENSE.md`); the
non-commercial condition follows the terms of the IUCN Red List, Living Planet Index and WDPA inputs,
and rows derived from the Living Planet Database stay under the Living Planet Index data terms.
The repository contains derived summaries only: no range polygons, no protected-area polygons
and no population time series are redistributed; the sources above must be credited when
values are reused.
