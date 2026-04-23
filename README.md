# profitable-app-profiles

A data analysis project that identifies profitable app profiles for a company building **free, ad-supported apps** on iOS and Android.

---

## Overview

The goal is to find app categories with the highest user demand on both the **Apple App Store** and **Google Play**, and recommend an app profile likely to succeed on both platforms.

Since the company's revenue comes from in-app ads, user volume is the key metric — more users means more ad impressions and higher revenue.

---

## Dataset

| Dataset | Source | Apps | Year |
|---|---|---|---|
| Google Play Store | Kaggle | ~10,000 | Aug 2018 |
| Apple App Store | Kaggle | ~7,000 | Jul 2017 |

Both datasets contain only free, English-language apps after cleaning.

---

## Project Structure

```
app_market_analysis.ipynb   ← main notebook
AppleStore.csv              ← iOS dataset
googleplaystore.csv         ← Android dataset
```

---

## Analysis Steps

1. **Load & Explore** — inspect shape, columns, and sample rows  
2. **Clean Data**
   - Remove one corrupted row (row 10472, Google Play)
   - Drop duplicate entries, keeping the highest-review version
   - Filter out non-English apps
   - Keep only free apps
3. **Genre Distribution** — frequency tables and bar charts for both platforms  
4. **Popularity Analysis** — average rating counts (iOS) and average installs (Android) by category  
5. **Visualizations** — 6 charts covering distribution, popularity, and a cross-platform comparison map  
6. **Recommendation** — data-backed app profile suggestion  

---

## Key Findings

- The App Store is dominated by games (58%), but practical categories like **Reference** and **Education** show higher average engagement
- Google Play is more balanced; **Books & Reference** and **Education** stand out as underserved but popular categories
- Communication, Social, and Video apps on Android have massive installs but are skewed by a few dominant players

---

## Recommendation

**Books & Reference** — specifically an interactive book companion app — is the most promising profile for both platforms. The category has genuine organic demand without being locked up by one unbeatable product.

---

## Tools Used

- Python 3
- `csv` (standard library)
- `matplotlib`
- `seaborn`

---

## How to Run

```bash
git clone https://github.com/your-username/app-market-analysis.git
cd app-market-analysis
pip install matplotlib seaborn
jupyter notebook app_market_analysis.ipynb
```

---

## Author

Mohamed — aspiring data scientist 
[LinkedIn](linkedin.com/in/mohamed-mostafa-m10) · [GitHub](https://github.com/MohamedYounes20)
