# Pakistan Real Estate Market Analytics (Zameen.com EDA)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python 3.10+](https://img.shields.io/badge/Python-3.10%2B-3776AB.svg)](https://www.python.org/)

An end-to-end **Exploratory Data Analysis (EDA) & Market Intelligence** study of Pakistan's real estate listings scraped from Zameen.com — covering fuzzy city normalization, area unit standardization, outlier treatment, engineered pricing metrics (`price_per_sqft`), and executive market visuals.

---

## Key Market Insights

- **Location & Asset Type Dominance**: City tier and property class (House vs. Apartment vs. Plot) are the primary structural drivers of valuation variance.
- **Core Inventory Segment**: Mid-range **5–10 Marla residential houses** account for the highest market liquidity and listing volume.
- **Urban Rental Shift**: High-density metropolitan markets show accelerating apartment demand relative to standalone homes.
- **Emerging Investment Corridors**: Secondary cities such as **Faisalabad** and **Multan** present attractive price-per-sqft entry points for growth-oriented investors.

---

## Project Structure

```text
pakistan-real-estate-eda/
├── data/
│   ├── zameen_raw.csv                        # Raw scraped Zameen.com listings
│   └── zameen_cleaned.csv                    # Cleaned & standardized analytical dataset
├── notebooks/
│   └── zameen_eda_final.ipynb                # Full data cleaning, fuzzy matching & EDA notebook
├── reports/
│   └── zameen_eda_insights_report.pdf        # Executive market insights report
├── visuals/                                  # Exported distribution, correlation & city-tier charts
│   ├── boxplot_price_pkr.png
│   ├── correlation_heatmap.png
│   ├── feature_distributions.png
│   ├── price_by_bedroom_bucket.png
│   ├── price_by_city_top10.png
│   └── price_by_property_type.png
├── requirements.txt
├── .gitignore
├── LICENSE                                   # MIT License
└── README.md
```

---

## Quick Start

```bash
git clone https://github.com/mirzahammad1/pakistan-real-estate-eda.git
cd pakistan-real-estate-eda

python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt

jupyter notebook notebooks/zameen_eda_final.ipynb
```

---

## License

This project is licensed under the [MIT License](LICENSE).
