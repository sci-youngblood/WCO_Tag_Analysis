# FIDELITY AND FLUX: Comparative Analysis of Marine Predator Residency
### Channel Islands National Marine Sanctuary (CINMS) — Acoustic Telemetry Project

**Author:** Morgan Youngblood  
**Affiliation:** University of Hawaiʻi at Hilo — Marine Science Program  
**Dataset span:** 2013–2024 (11 years)  
**Status:** Analysis complete

---

## Overview

This repository contains the full analysis pipeline for a multi-species acoustic 
telemetry study conducted within the Channel Islands National Marine Sanctuary (CINMS). 
The project quantifies movement patterns, seasonal residency, and habitat fidelity 
across 7 threatened and vulnerable marine predator species using an 11-year longitudinal 
detection dataset.

Key metrics include residency index (RI) calculations, maximum daily displacement, 
seasonal fidelity scoring, and species-specific spatial summaries across four Northern 
Channel Islands.

---

## Dataset

| Parameter | Value |
|---|---|
| Transmitters processed | 277 (224 distinct individuals) |
| Species analyzed | 7 (threatened/vulnerable marine predators) |
| Receiver array | 13 Innovasea VR2Tx/VR2AR units, 4 Northern Channel Islands |
| Detection records | ~11-year longitudinal dataset (2013–2024) |
| Collaborative network | West Coast universities and research institutions |

> **Note:** Raw detection data (`.csv`) are excluded from this repository due to 
> file size and data-sharing agreements. Scripts are fully documented and reproducible 
> given access to source data.

---

## Repository StructureWCO_Tag_Analysis/
├── scripts/
│   ├── manuscript_analysis.Rmd        # Primary analysis — figures, stats, residency index
│   ├── White_Bat_Products.rmd         # Species-specific outputs: White Shark & Bat Ray
│   ├── Cleaning WCO Data and adding Tag info.rmd  # QA/QC and tag metadata integration
│   ├── Kickback_Tag_Data.Rmd          # Collaborator data exchange pipeline
│   ├── adescript.Rmd                  # Array descriptive statistics
│   └── Update_Tag_ID.rmd              # Tag ID reconciliation across receiver networks
├── data/                              # Raw data excluded via .gitignore (see note above)
└── outputs/                           # Derived summary tables and figures---

## Technical Stack

- **Language:** R
- **Core packages:** `tidyverse`, `ggplot2`, `sf`, `terra`, `geosphere`, `FSA`, `lubridate`
- **Hardware:** Innovasea VR2Tx / VR2AR acoustic receivers, VUE software
- **Spatial reference:** UTM Zone 11N / WGS84

---

## Key Findings

- Quantified broad-scale spatial patterns and seasonal fidelity across 7 predator species
- Calculated maximum daily displacement of **45.5 km** for juvenile White Sharks
- Identified critical aggregation sites for White Sharks, Giant Sea Bass, and Leopard Sharks
- Demonstrated species-specific residency gradients across the Northern Channel Islands

---

## Acknowledgments

This project was made possible through a highly collaborative network of researchers 
and institutions across the U.S. West Coast. Tagging data, field support, and analytical 
contributions were provided by collaborators at multiple universities and research 
institutions. Individual contributor detection datasets are not included in this public 
repository out of respect for data-sharing agreements.

Special thanks to R. Freedman for mentorship and guidance throughout this project.

---

## License

Code in this repository is released under the [MIT License](LICENSE).  
Data are not included and remain subject to the data-sharing agreements of the 
contributing institutions.
