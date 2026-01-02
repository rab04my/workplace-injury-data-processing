# Workplace Injury Multi-Dataset Analysis

This repository contains Python analysis code for harmonizing and exploring **five U.S. workplace injury datasets** spanning **2015–2024** (selected range for this study), totaling **~7.5M records**. The notebook processes raw data, performs text classification on injury narratives, generates visualizations, and computes dataset completeness metrics.

## 📊 Datasets Included

| Dataset   | Source                                                                 | Records | Focus                                      |
|-----------|------------------------------------------------------------------------|---------|--------------------------------------------|
| OSHA SIR  | [U.S. Dept. Labor, OSHA](https://www.osha.gov/ords/imis/accidentsearch.html) | 97K     | Severe injuries (hospitalization, amputation, eye loss) |
| OSHA ITA  | [U.S. Dept. Labor, OSHA](https://www.osha.gov/ords/imis/accidentsearch.html) | 1.64M   | Recordable cases w/ narratives             |
| TX SV2    | [Texas DWC](https://www.tdi.texas.gov/wc/sv2/index.html)               | 5.4M    | Medical billing transactions               |
| OR WC     | [Oregon DCBS](https://www.oregon.gov/dcbs/analytics/Pages/data-requests.aspx) | 170K    | Workers' comp claims                        |
| NY WC     | [NY WCB](https://www.wcb.ny.gov/content/main/Research/Research-Statistics.jsp) | 266K    | Workers' comp claims                        |

**Raw data sources** (public access required):
- OSHA SIR/ITA: [OSHA Injury Tracking Application](https://www.osha.gov/ords/imis/accidentsearch.html)
- TX SV2: [Texas Division of Workers' Compensation](https://www.tdi.texas.gov/wc/sv2/index.html)
- OR WC: [Oregon DCBS Data Requests](https://www.oregon.gov/dcbs/analytics/Pages/data-requests.aspx)
- NY WC: [NY Workers' Compensation Board](https://www.wcb.ny.gov/content/main/Research/Research-Statistics.jsp)

## 🎯 Key Features

- **Data harmonization** across datasets (dates, NAICS, injury types, body parts, events)
- **NLP text classification** of injury narratives using fuzzy matching and TF-IDF
- **Temporal analysis** (monthly/yearly trends, heatmap by month/day-of-week)
- **Visualizations**: Top industries, injury types, event distributions, hospitalization rates
- **Cross-dataset comparisons** (event/body part matrices, industry rankings)

## 📁 Repository Structure

```
├── workplace_injury_data_processing_and_eda.ipynb   # Main analysis notebook (attached file)
├── outputs/                                         # Generated figures & tables (if included)
│   ├── *.csv
│   └── *.jpg
│   └── ...
├── README.md                                        # This file
└── data/                                            # Processed CSVs (if <100MB total)
    ├── ITA_PROCESSED.csv
    ├── SIR_PROCESSED.csv
    └── ...
```

**Note**: Raw data files are large (~GBs) and **not included** due to GitHub limits. Download from source URLs above and run the notebook locally.

## 📝 Citation

Cite as:
```
Workplace Injury Multi-Dataset Processing and Analysis (2026). GitHub repository.
https://github.com/[username]/workplace-injury-analysis
```

## 🙋 Issues & Contributions

Report bugs or suggest improvements via Issues. Pull requests welcome!

***
