# Water (e)Quality: Evaluating Equity and Efficacy of LA County's Stormwater Capture Projects

A Bren School of Environmental Science & Management Master's Group Project (2025-2026)

## About This README

This README serves as the central navigation guide for the Water (e)Quality project repositories. It documents the structure of both the main shared repository and each team member's individual repository, describes the data sources and file organization conventions used across the project, and provides context on each team member's analytical focus area. Whether you are a team member onboarding to the project, a collaborator seeking to understand how the work is organized, or a reviewer exploring the codebase, this document is the starting point for understanding how the project is structured and where to find specific analyses, data, and outputs.

## Project Overview

This project evaluates the effectiveness and equitable distribution of stormwater capture projects in Los Angeles County, analyzing their impact on water quality at beaches and rivers. We utilize a decade of fecal indicator bacteria (FIB) data to understand long-term trends and make recommendations for future stormwater infrastructure investments.

**Client:** Annelisa Moe, Heal the Bay  
**Faculty Advisor:** Dr. Naomi Tague  
**External Advisors:** Dr. Arturo Keller, Jenny Newman

## Team Members & Repositories

Each team member maintains their own repository for individual analyses and workflows. All repositories follow the same structure and data management guidelines.

### Team Repositories

- **Claire Anderson** - [Repository Link](https://github.com/Water-eQuality/Claire-Anderson)
- **Samuel Cervantes** - [Repository Link](https://github.com/Water-eQuality/Samuel-Cervantes) — contains all materials for the cost and equity analysis
- **Nico Gavigan** - [Repository Link](https://github.com/Water-eQuality/Nico-Gavigan) — contains all materials for the Stormwater Capture Project Efficacy analysis
- **Lili Khosravi** - [Repository Link](https://github.com/Water-eQuality/Lili-Khosravi-)
- **Tina Tran** - [Repository Link](https://github.com/Water-eQuality/Tina-Tran) — contains all materials for the FIB and Precipitation Analysis

### Main Project Repository
- **Water (e)Quality Main** - [Repository Link](https://github.com/Water-eQuality/Water-eQuality-Data)

## Repository Structure

### Individual Member Repositories

Each team member's repository follows this structure:

```
[Member-Name]/
├── data/                       # Data files and inputs for individual analyses
├── docs/                       # Documentation and reference materials
├── outputs/                    # Generated figures, maps, and analysis outputs
├── scripts/                    # Analysis, cleaning, and visualization scripts (R, Python)
├── .gitignore                  # Git ignore rules
├── README.md                   # Repository documentation
└── [Member-Name].Rproj         # RStudio project file
```

### Main Project Repository

The main repository houses shared data, final analyses, and project deliverables:

```
Water-eQuality-Data/
├── data/
│   ├── raw/                                        # Original, unmodified data files
│   │   ├── CalEnviroScreen/                        # CalEnviroScreen 4.0 data
│   │   ├── beach_monitoring_location_data/         # Beach monitoring site locations
│   │   ├── precipitation/                          # Precipitation station data
│   │   ├── public_parks/                           # County parks and open space data
│   │   ├── shapefiles/                             # Spatial boundary files
│   │   ├── wramps/                                 # WRAMPS stormwater project data
│   │   ├── beach_monitoring_data_start_dates.csv
│   │   ├── countywide_parks_and_open_space.csv
│   │   ├── la_major_rivers.zip
│   │   ├── la_public_health_beach_testing_locations_master_copy.csv
│   │   ├── national_priorities_list_boundaries.zip
│   │   ├── raw_master_beach_data_2014_2024.csv
│   │   ├── storm_drains_2024.csv
│   │   └── tree_canopy_coverage.zip
│   ├── processed/                                  # Cleaned and analysis-ready datasets
│   │   ├── beach_data/
│   │   ├── parcels/
│   │   ├── precipitation/
│   │   ├── recommended_sites/
│   │   ├── river_data/
│   │   └── wramps/
│   └── archive/                                    # Superseded or legacy data files
│       ├── htb_fib_all_clean.csv
│       ├── htb_fib_loc_na.csv
│       ├── htb_rain_clean.csv
│       ├── htb_tbl_california_rain.xlsx
│       └── htb_tbl_location.xlsx
├── figures/                                        # Generated figures
│   ├── beach_graph_total_samples/
│   ├── beach_zero/
│   ├── fib_timeseries_log/
│   ├── fib_timeseries_no_log/
│   ├── summer_river_figures/
│   └── full_data_heatmap.png
├── outputs/
│   └── figures/                                    # Polished output figures
├── scripts/                                        # Analysis and processing scripts
│   ├── analysis/
│   ├── data_cleaning/
│   ├── lili/
│   │   ├── exceedance_plots.R
│   │   └── lili_exceedance_analysis.qmd
│   └── tina/
│       └── sample_count_figures.qmd
├── .gitignore
├── README.md
├── Watershed Control Measures Completed Tab...     # Watershed control measures reference table
└── water_equality_gp.Rproj                         # RStudio project file
```

## Project Objectives

1. **Ten-Year Water Quality Analysis**: Conduct a comprehensive analysis of Los Angeles County beach and river fecal indicator bacteria (FIB) data (2014-2024) to identify long-term trends in water quality.

2. **Stormwater Capture Project Impact Assessment**: Determine how stormwater capture projects impact downstream water quality through before-and-after analyses.

3. **Future Investment Recommendations**: Identify priority areas in LA County for new stormwater capture project implementation, considering both efficacy and equity.

## Significance

This project supports critical advocacy for improving stormwater regulation in LA County ahead of the MS4 permit revision in summer 2026. Results will inform Heal the Bay's recommendations to the LA Regional Water Quality Control Board for enhanced regulations and prioritized project implementation.

Urban runoff is the primary source of pollution degrading LA County's surface water quality. With 70% of rainfall occurring January-March and extensive impervious surfaces, stormwater carries pollutants directly to rivers and beaches, causing ~3.5 million sick days annually in California due to contaminated beach waters.

## Contact

For questions about this project, please contact:
- **Bren School Group Projects**: Lili Khosravi (lkhosravi@bren.ucsb.edu)

## Acknowledgments

This project is conducted in partnership with Heal the Bay and supported by the Bren School of Environmental Science & Management at UC Santa Barbara.

---

*Last Updated: May 2026*
