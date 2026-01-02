# Workplace Injury Multi-Dataset Analysis

This repository contains Python analysis code for harmonizing and exploring **five U.S. workplace injury datasets** spanning **2015–2024** (selected range for this study), totaling **~7.5M records**. The notebook processes raw data, performs text classification on injury narratives, generates visualizations, and computes dataset completeness metrics.

## 📊 Datasets Included

| Dataset   | Source                                                                 | Records | Focus                                      |
|-----------|------------------------------------------------------------------------|---------|--------------------------------------------|
| OSHA SIR  | [U.S. Dept. Labor, OSHA](https://www.osha.gov/severe-injury-reports) | 97K     | Severe injuries (hospitalization, amputation, eye loss) |
| OSHA ITA  | [U.S. Dept. Labor, OSHA](https://www.osha.gov/Establishment-Specific-Injury-and-Illness-Data) | 1.64M   | Recordable cases w/ narratives             |
| TX SV2    | [Texas Dept. of Insurance](https://www.tdi.texas.gov/wc/index.html)               | 5.4M    | Medical billing transactions               |
| OR WC     | [Oregon Worker's Compensation Division](https://wcd.oregon.gov/Pages/index.aspx) | 170K    | Workers' comp claims                        |
| NY WC     | [NY Workers’ Compensation Board](https://www.wcb.ny.gov/) | 266K    | Workers' comp claims                        |

**Raw data sources** (public access required):
- OSHA SIR: [Severe Injury Dashboard](https://www.osha.gov/severe-injury-reports)
- OSHA ITA: [OSHA Injury Tracking Application (ITA) Data](https://www.osha.gov/Establishment-Specific-Injury-and-Illness-Data)
- TX SV2: [Texas Institutional Medical Billing Services (SV2) Detail Information](https://data.texas.gov/dataset/Institutional-Medical-Billing-Services-SV2-Detail-/tuuc-49gz/about_data)
- OR WC: [Oregon Workers' Compensation Record Level Claims](https://catalog.data.gov/dataset/oregon-workers-compensation-record-level-claims)
- NY WC: [NY State Workers' Compensation Injury Claims](https://www.kaggle.com/datasets/thedevastator/new-york-state-workers-compensation-injury-claim)

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
