# Healthcare Analytics Executive Dashboard

An executive-level dashboard built from a Python analysis of a healthcare dataset (54,966 records after de-duplication). It answers one question: **what does hospital management need to know?**

![Dashboard preview](docs/dashboard-preview.png)

## Live view
Download `dashboard.html` and open it in any browser (works offline). To host it, enable GitHub Pages and rename the file to `index.html`.

## Key findings
- **Balanced demand:** all 6 medical conditions account for 16.6%–16.8% of patients each; no single condition dominates.
- **No payer dependency:** 5 insurers each cover about 20% of patients (Cigna highest at 11,139).
- **Stable billing:** average billing is about $25.6K per patient, and monthly averages stay between about $24.9K and $26.3K.
- **Age does not drive cost:** patients aged 60+ average $25,564, in line with the overall average.
- **Emergency load:** 18,102 admissions (32.9%) are emergencies; July is the busiest month (1,573), February the lightest (1,452).
- **Review queues:** 6,038 emergency patients have abnormal test results, and 5,497 patients sit in the top 10% of billing.

## Dashboard contents
- KPI cards: total patients, average billing, average age, emergency admissions, insurers, conditions
- Executive summary and management takeaways
- Interactive charts with tooltips
- Filters: Medical Condition, Insurance Provider, Reset

## Project structure
```
├── dashboard.html          # self-contained executive dashboard
├── notebook/
│   └── Healthcare_Analysis.ipynb   # data cleaning and analysis (Python)
└── docs/
    └── dashboard-preview.png
```

## Tools
Python, Pandas, Jupyter Notebook for the analysis. The dashboard is built with HTML/CSS and Chart.js (bundled inside the file, so it needs no internet).

## Notes
- The dataset has no Department column, so no department filter is included.
- The dashboard presents aggregated results from the notebook; it does not contain patient-level data.

## Author
**Om Kadam** – Data Analyst | [LinkedIn](https://linkedin.com/in/om-kadam-308b802b7)
