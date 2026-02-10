# Agricultural Data Science Portfolio - Soil Intensive

**Sydney Seiter** | Computational Agronomist & Data Scientist  
📧 Contact: [sydney.seiter22@gmail.com] | 🔗 LinkedIn: [https://www.linkedin.com/in/sydney-seiter-309475277/]

---

## Overview

This portfolio showcases data science and database management skills applied to real-world agricultural research and production operations. Drawing from hands-on experience in commercial vegetable farming and field research across the Southeastern United States, these projects demonstrate the intersection of agricultural expertise and computational analysis.

### Background

- **M.S. Data Science**, Eastern University
- **B.S. Plant & Microbial Biology**, NC State University
- **Field Experience**: Commercial vegetable production operations (potato, sweet potato, spinach, watermelon) and multi-site agricultural research trials
- **Geographic Expertise**: Eastern North Carolina, South Carolina, and Georgia production regions

---

## Projects

### 📊 Project 1: Multi-Site Soil Data QA/QC Pipeline

**File:** `soil_data_qa_standardization_2026.ipynb`

#### Summary
Demonstrates data quality assurance protocols for integrating soil test results from multiple laboratories across research sites. Addresses real-world challenges in multi-site agricultural research: heterogeneous data formats, different laboratory methods, and varying quality control standards.

#### Research Context
- **Sites**: Eastern NC (Johnston County), Aiken SC, Donalsonville GA
- **Challenge**: Three different soil testing laboratories with different P extraction methods (Mehlich-3 vs Mehlich-1)
- **Approach**: Standardization pipeline with agronomically-meaningful validation rules

#### Skills Demonstrated
- **Data Integration**: Combining datasets with inconsistent formats and nomenclature
- **Domain Knowledge**: Understanding soil chemistry (pH patterns, CEC-OM relationships, P method differences)
- **Quality Control**: Implementing validation rules based on agronomic ranges
- **Data Visualization**: QC dashboards for multi-site comparisons
- **Documentation**: Full audit trails and processing logs

#### Key Features
- ✅ Automated detection of 6+ data quality issues
- ✅ Standardization of units, depth measurements, and column names
- ✅ QA flag system (PASS/FAIL/REVIEW) with specific failure reasons
- ✅ Phosphorus extraction method tracking (critical for interpretation)
- ✅ Database-ready exports with comprehensive data dictionaries

---

### 🌱 Project 2: Sweet Potato Variety Trial Analysis

**File:** `field_trial_statistical_analysis.ipynb`

#### Summary
Multi-site statistical analysis of sweet potato variety performance across three Southeastern production regions. Demonstrates experimental design, ANOVA, and practical decision-making tools for grower recommendations.

#### Trial Design
- **Sites**: Eastern NC, Aiken SC, Donalsonville GA
- **Varieties**: Covington, Beauregard, Evangeline, Orleans
- **Design**: Randomized Complete Block Design (4 blocks × 3 sites × 2 years)
- **Metrics**: Total yield, marketable yield, quality grades (Jumbo, #1, #2, Culls)

#### Skills Demonstrated
- **Experimental Design**: RCBD with proper blocking for field variability
- **Statistical Analysis**: Two-way ANOVA, Tukey HSD post-hoc tests, effect size calculations
- **Agricultural Expertise**: Commercial grading standards, realistic yield ranges, quality metrics
- **Data Visualization**: Publication-quality graphics for extension/industry audiences
- **Stakeholder Communication**: Translating statistics into grower-friendly recommendations

#### Key Features
- ✅ Realistic variety characteristics based on industry standards
- ✅ Site-specific performance patterns (soil type, climate effects)
- ✅ Year-to-year stability analysis
- ✅ Yield × Quality decision matrix for variety selection
- ✅ Extension-ready summary with economic considerations

---

### 🗄️ Project 3: Vegetable Farming Operations Database

**File:** `database_design_etl_pipeline.ipynb`

#### Summary
Production-grade relational database system for managing commercial vegetable farming operations across multiple crops and locations. Demonstrates database architecture, regulatory compliance tracking, and operational analytics.

#### Database Scope
- **Crops**: Potato, Sweet Potato, Spinach, Watermelon
- **Locations**: Eastern NC, Aiken SC, Donalsonville GA
- **Operations**: Planting, IPM applications, harvest, quality grading, product tracking

#### Database Schema (10 Core Tables)
1. **crops** - Crop master data and growing characteristics
2. **fields** - Production areas with soil types and irrigation
3. **plantings** - Planting records with varieties and expected harvest dates
4. **ipm_applications** - Pesticide/fungicide tracking with EPA registrations
5. **field_operations** - Tillage, cultivation, equipment usage
6. **harvest_records** - Harvest timing, crew, bins, total weight
7. **quality_inspections** - Grade distributions and defect tracking
8. **products** - Packaged products with lot numbers and GTINs
9. **weather_log** - Daily weather observations
10. **workers** - Crew management and applicator certifications

#### Skills Demonstrated
- **Database Design**: Normalized relational schema with foreign key constraints
- **Regulatory Compliance**: PHI (Pre-Harvest Interval) and REI (Re-Entry Interval) tracking
- **Quality Control**: Crop-specific grading systems (sweet potato grades, watermelon Brix, spinach bolting)
- **Traceability**: Full chain from planting through packaged product
- **SQL Proficiency**: Complex queries with joins, aggregations, and compliance verification
- **Production Analytics**: Yield analysis, quality distributions, harvest timelines

#### Key Features
- ✅ IPM application tracking with actual EPA-registered products
- ✅ Automated PHI compliance verification (100% compliant in demo)
- ✅ Multi-crop quality grading (handles root, leaf, and fruit vegetables)
- ✅ Crew and worker management with certification tracking
- ✅ Production dashboards for operational decision-making
- ✅ Exportable reports for regulatory compliance and record-keeping

---

## Technical Stack

### Languages & Libraries
- **Python 3.8+**
- **pandas** - Data manipulation and analysis
- **numpy** - Numerical computing
- **matplotlib/seaborn** - Data visualization
- **scipy** - Statistical analysis
- **statsmodels** - ANOVA and post-hoc tests
- **sqlite3** - Database management (production would use PostgreSQL)

### Tools & Platforms
- **Jupyter/Google Colab** - Interactive development
- **Git/GitHub** - Version control
- **SQL** - Database queries and analytics

---

## Running the Notebooks

### Requirements
```bash
pip install pandas numpy matplotlib seaborn scipy statsmodels
```

### Google Colab (Recommended)
1. Upload notebook to Google Colab
2. Run all cells (no additional setup required)
3. Outputs save to current directory or Google Drive (configurable)

### Local Jupyter
```bash
jupyter notebook soil_data_qa_standardization_2026.ipynb
```

### Configuration
Each notebook includes a setup cell for choosing output location:
- **Option 1**: Current directory (default)
- **Option 2**: Dedicated output folder
- **Option 3**: Google Drive (auto-mount in Colab)

---

## Project Outputs

### Notebook 1 Outputs
- `soil_qc_dashboard.png` - Multi-site quality control visualizations
- `soil_data_standardized.csv` - Cleaned and standardized data
- `soil_data_dictionary.csv` - Metadata and column descriptions
- `processing_log.json` - Full audit trail of transformations

### Notebook 2 Outputs
- `sweetpotato_variety_comparison.png` - Variety performance across sites
- `year_to_year_stability.png` - Temporal consistency analysis
- `variety_decision_matrix.png` - Yield × Quality decision tool
- `sweetpotato_trial_results.csv` - Complete trial dataset

### Notebook 3 Outputs
- `vegetable_farming_operations.db` - SQLite database with all production data
- `production_dashboard.png` - Operational analytics visualizations
- `season_2025_production_report.csv` - Comprehensive season summary
- `ipm_application_log_2025.csv` - Regulatory compliance report
- `database_schema_documentation.csv` - Complete schema documentation

---

## Key Insights & Assumptions

### Realistic Agricultural Context
All projects use realistic assumptions grounded in commercial production:

- **Yield Ranges**: Sweet potato yields of 18,000-21,000 lbs/acre align with Southeast industry standards
- **Quality Grades**: 35-40% jumbo, 42-48% #1 grade, 7-10% culls reflect commercial operations
- **Regional Patterns**: pH gradients (acidic NC → neutral GA), organic matter trends match soil types
- **IPM Products**: Actual EPA-registered products (Bravo, Admire Pro, Command, Manzate) with correct PHI/REI intervals
- **Crop Timing**: Planting and harvest windows appropriate for Southeast climate

### Data Quality
- Notebook 1: ~95% QA pass rate (realistic for multi-site research)
- Notebook 2: Variety effects based on published literature and industry knowledge
- Notebook 3: 100% PHI compliance (best practices demonstration)

### Limitations
- Data is simulated but reflects real-world patterns and constraints
- Does not include extreme events (hurricanes, equipment failures, market disruptions)
- Assumes proper agronomic management and favorable growing conditions

---

## Skills Highlights

### Data Science
✅ Multi-site data integration and standardization  
✅ Statistical analysis (ANOVA, post-hoc tests, effect sizes)  
✅ Database design and normalization  
✅ ETL pipeline development  
✅ Quality control systems  
✅ Data visualization for diverse audiences  

### Agricultural Expertise
✅ Commercial vegetable production (potato, sweet potato, spinach, watermelon)  
✅ Field trial design and analysis  
✅ Soil chemistry and fertility  
✅ IPM and regulatory compliance  
✅ Quality grading systems  
✅ Southeast production regions  

### Technical Skills
✅ Python (pandas, numpy, scipy, statsmodels)  
✅ SQL (complex queries, joins, aggregations)  
✅ Database design (relational schemas, normalization)  
✅ Data validation and QA protocols  
✅ Jupyter notebooks and reproducible workflows  
✅ Git version control  

---

## Applications

These skills directly support:

- **Research Organizations**: Multi-site trial coordination, data management, statistical analysis
- **Agricultural Technology**: Production databases, precision agriculture data pipelines
- **Food Safety/Compliance**: Traceability systems, regulatory reporting, PHI/REI tracking
- **Extension/Consulting**: Variety recommendations, production analytics, grower decision tools
- **Agribusiness**: Supply chain data, quality control systems, operational analytics

---

## About the Author

Sydney Seiter is a computational agronomist combining hands-on agricultural experience with data science expertise. With a background spanning commercial vegetable production, field research, and database development, Sydney specializes in building data systems that bridge the gap between field operations and analytical insights.

**Experience includes:**
- Commercial vegetable farming operations across Eastern NC, SC, and GA
- Multi-site agricultural field trials
- Database development for production tracking and compliance
- Consulting on agricultural data systems (U.S. Composting Council)

---

## License

This portfolio is shared for educational and professional demonstration purposes. Code is available under MIT License. Data is simulated for demonstration purposes.

---

## Contact

For questions, collaborations, or opportunities:
- **Email**: [sydney.seiter22@gmail.com]
- **LinkedIn**: [https://www.linkedin.com/in/sydney-seiter-309475277/]
- **GitHub**: [github.com/Buffy686]

---

*Last Updated: February 2026*
