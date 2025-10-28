# Water (e)Quality: Evaluating Equity and Efficacy of LA County's Stormwater Capture Projects

A Bren School of Environmental Science & Management Master's Group Project (2025-2026)

## Project Overview

This project evaluates the effectiveness and equitable distribution of stormwater capture projects in Los Angeles County, analyzing their impact on water quality at beaches and rivers. We utilize a decade of fecal indicator bacteria (FIB) data to understand long-term trends and make recommendations for future stormwater infrastructure investments.

**Client:** Annelisa Moe, Heal the Bay  
**Faculty Advisor:** Dr. Naomi Tague  
**External Advisors:** Dr. Arturo Keller, Jenny Newman

## Team Members & Repositories

Each team member maintains their own repository for individual analyses and workflows. All repositories follow the same structure and data management guidelines.

### Team Repositories

- **Claire Anderson** - [Repository Link](https://github.com/Water-eQuality/Claire-Anderson)
- **Samuel Cervantes** - [Repository Link](https://github.com/Water-eQuality/Samuel-Cervantes)
- **Nico Gavigan** - [Repository Link](https://github.com/Water-eQuality/Nico-Gavigan)
- **Lili Khosravi** - [Repository Link](https://github.com/Water-eQuality/Lili-Khosravi-)
- **Tina Tran** - [Repository Link](https://github.com/Water-eQuality/Tina-Tran)

### Main Project Repository
- **Water (e)Quality Main** - [Repository Link](https://github.com/Water-eQuality/Water-eQuality-Data)

## Project Objectives

1. **Ten-Year Water Quality Analysis**: Conduct a comprehensive analysis of Los Angeles County beach and river fecal indicator bacteria (FIB) data (2014-2024) to identify long-term trends in water quality.

2. **Stormwater Capture Project Impact Assessment**: Determine how stormwater capture projects impact downstream water quality through before-and-after analyses.

3. **Future Investment Recommendations**: Identify priority areas in LA County for new stormwater capture project implementation, considering both efficacy and equity.

## Repository Structure

```
water-equality/
├── data/
│   ├── raw/                    # Original, unmodified data files
│   │   ├── beach_fib/         # Beach water quality data (1995-2024)
│   │   ├── river_fib/         # River monitoring data (2014-present)
│   │   ├── precipitation/     # AccuWeather and NowCast rainfall data
│   │   └── stormwater_projects/ # SWCP inventory and metadata
│   ├── processed/             # Cleaned and processed datasets
│   └── metadata/              # Data dictionaries and documentation
├── scripts/
│   ├── data_cleaning/         # Data processing and cleaning scripts
│   ├── analysis/              # Analysis scripts (R, Python)
│   └── visualization/         # Plotting and mapping scripts
├── outputs/
│   ├── figures/               # Generated plots and visualizations
│   ├── maps/                  # GIS maps and spatial analyses
│   └── reports/               # Analysis reports and summaries
├── docs/
│   ├── interim_report.pdf     # Project interim report
│   └── methods/               # Detailed methodology documentation
└── README.md
```

## Key Data Sources

### Water Quality Data
- **Beach FIB Data** (1995-2024): Total coliform, E. coli, fecal coliform, and enterococcus concentrations from California Water Board
- **River FIB Data** (2014-present): Weekly monitoring data from Heal the Bay, including turbidity and temperature measurements

### Precipitation Data
- AccuWeather and NowCast station data (2014-present)
- Long Beach and LAX rainfall stations

### Stormwater Infrastructure
- **WRAMPS 2.0**: LA County Stormwater Capture Dashboard with 662+ projects
- **Safe Clean Water Program Portal**: SCWP-funded project locations, types, and capacity data
- **Completed Projects Dataset**: Upper LA River watershed projects from WMMS 2.0 metadata

### Geospatial Data
- LA County Enterprise GIS (watersheds, subwatersheds, land use)
- LADPW Storm Drain System geodatabase
- CalEnviroScreen 4.0 (census tract pollution and demographic data)

## Key Definitions

### Best Management Practice (BMP) Types
- **Bioretention**: Filters stormwater through plants, soil, sand, and gravel
- **Biofiltration**: Uses microorganisms to break down pollutants
- **Infiltration Well**: Captures runoff before reaching water bodies
- **Treatment Facility**: Intercepts and treats stormwater for reuse
- **Sanitary Sewer Diversion**: Diverts stormwater to treatment plants

### Water Quality Metrics
- **FIB (Fecal Indicator Bacteria)**: Includes E. coli, fecal coliform, total coliform, and enterococcus
- **Exceedance**: Water sample exceeding California AB 411 standards
  - Total coliform: 10,000 MPN/100 mL (single sample)
  - Fecal coliform: 400 MPN/100 mL (single sample)
  - Enterococcus: 104 MPN/100 mL (single sample)
  - E. coli: 235 MPN/100 mL (single sample)

### Seasons
- **Dry Weather Season**: May - October
- **Wet Weather Season**: November - April

### Communities
- **Disadvantaged Community (DAC)**: Census block groups with median household income <80% of California statewide median

## Analysis Methods

### 1. FIB Trend Analysis
- Ten-year temporal trends at individual monitoring sites
- Wet vs. dry season comparisons
- Exceedance frequency and peak concentration analysis
- Geographic patterns (upper vs. lower watershed)

### 2. Precipitation-FIB Relationship
- Storm event impact on water quality
- First flush analysis
- Antecedent dry period effects

### 3. Stormwater Capture Project Efficacy
- Before-and-after analysis of project implementation
- Project type comparison (bioretention, infiltration wells, etc.)
- Volume captured vs. water quality improvements

### 4. Equity Assessment
- Distribution of projects across DACs vs. non-DACs
- Co-benefits analysis (flood reduction, green space, heat island effect)
- Beach closure impacts on vulnerable communities

## Technologies & Tools

- **Programming**: R, Python
- **GIS**: ArcGIS, QGIS
- **Models**: WMMS 2.0, WRAMPS 2.0, PLET
- **Data Management**: Git, GitHub
- **Visualization**: ggplot2, matplotlib, Tableau

## Project Timeline

- **Fall 2025**: Data collection, cleaning, and preliminary analysis
- **Winter 2026**: Complete analysis, modeling, and draft report
- **Spring 2026**: Final report, executive summary, and presentations (April 2026)

## Significance

This project supports critical advocacy for improving stormwater regulation in LA County ahead of the MS4 permit revision in summer 2026. Results will inform Heal the Bay's recommendations to the LA Regional Water Quality Control Board for enhanced regulations and prioritized project implementation.

Urban runoff is the primary source of pollution degrading LA County's surface water quality. With 70% of rainfall occurring January-March and extensive impervious surfaces, stormwater carries pollutants directly to rivers and beaches, causing ~3.5 million sick days annually in California due to contaminated beach waters.

## Collaborative Workflow

### Repository Structure
This project uses a **distributed repository model** where:
- **Main Repository**: Houses shared data, final analyses, and project deliverables
- **Individual Repositories**: Each team member maintains their own repo for exploratory analysis, development, and testing

### Working Across Repositories

1. **Clone the main repository** for access to shared datasets and documentation
   ```bash
   git clone https://github.com/Water-eQuality/Water-eQuality-Data.git
   ```

2. **Use your individual repository** for:
   - Exploratory data analysis
   - Testing new methods
   - Developing visualizations
   - Draft analyses and scripts

3. **Contribute to main repository** by:
   - Creating pull requests for finalized code
   - Adding polished visualizations to `outputs/`
   - Updating shared documentation
   - Contributing to analysis reports

### Best Practices for Collaboration
- **Sync regularly**: Pull updates from main repo frequently
- **Document everything**: Clear comments in code and README updates
- **Coordinate on Slack/Trello**: Discuss before major changes to main repo
- **Code reviews**: Have at least one team member review pull requests
- **Consistent naming**: Follow the data management guidelines across all repos

### File Naming Conventions
- Use descriptive names: `beach_fib_2014-2024_cleaned.csv`
- Include dates: `YYYY-MM-DD` or `YYYYMMDD`
- No spaces (use underscores or hyphens)
- Use lowercase for consistency

### Version Control
- Commit frequently with clear messages
- Never commit raw data files >100MB (use Git LFS if needed)
- Document all data transformations in scripts

### Data Privacy
- Do not commit sensitive or unpublished data
- Follow Heal the Bay's data sharing agreements
- Coordinate with client before sharing results publicly

## Contact

For questions about this project, please contact:
- **Bren School Group Projects**: Lili Khosravi (lkhosravi@ucsb.edu)
- **Heal the Bay**: Annelisa Moe

## Acknowledgments

This project is conducted in partnership with Heal the Bay and supported by the Bren School of Environmental Science & Management at UC Santa Barbara.

---

*Last Updated: October 2025*
