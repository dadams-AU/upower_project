# Oil & Gas Extraction Impacts Database

This repository supports a research project examining the dual impacts of oil and gas (O&G) extraction across U.S. counties between 2006 and 2024. Our central hypothesis is that O&G activity produces both temporary economic benefits and longer-term environmental and social harms, with outcomes shaped by regulatory, economic, and production-stage context.

## 📌 Project Aims

1. **Community Change**  
   Analyze how O&G production influences county-level economic indicators, demographics, local government finance, and environmental contaminants.

2. **Public Health Outcomes**  
   Evaluate the relationship between O&G production and health outcomes, including asthma, cancer, and substance use disorder, moderated by production stage.

3. **Regulatory Context**  
   Assess how enforcement patterns and state-level policies shape worker and community health outcomes.

4. **Equity and Spatial Disparities** *(Planned extension)*  
   Examine spatial disparities and equity implications across disproportionately affected communities.

---

## 🗃️ Repository Structure

```
project-root/
├── notebooks/                # Jupyter notebooks for setup and analysis
├── sql/                     # SQL scripts for schema setup
├── data/                    # Raw and processed datasets (gitignored)
├── scripts/                 # Python scripts for data collection/loading
├── README.md
└── requirements.txt         # Project dependencies
```

---

## ⚙️ Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/oil-gas-impacts-db.git
   cd oil-gas-impacts-db
   ```

2. Set up the PostGIS database:

   - Ensure PostgreSQL + PostGIS is installed and running
   - Edit the database credentials in `notebooks/init_postgis_db.ipynb`
   - Run the notebook to create tables

3. Install Python dependencies:

   ```bash
   pip install -r requirements.txt
   ```

---

## 📥 Data Sources

| Domain                     | Source                                         |
|---------------------------|------------------------------------------------|
| Economic & Demographic    | ACS, BEA, QCEW, IRS SOI                        |
| Local Government Finance  | Census of Governments, PA Department of Rev.  |
| Environmental Quality     | TRI, AQS, CAMD, NWIS, FracFocus, NASA/NOAA    |
| Health Outcomes           | CDC WONDER, BRFSS, State Health Depts         |
| Regulatory Data           | TRRC, COGCC, NCSL, IOGCC                       |
| Methane Emissions         | EPA Gridded Methane, MethaneSAT, GHGRP        |

---

## 📄 License

MIT License. See `LICENSE` file for details.

---

## 👨‍🔬 Maintainer

David P. Adams  
California State University, Fullerton  
[dadams.io](https://dadams.io)
