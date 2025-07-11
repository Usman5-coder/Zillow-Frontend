# 🏠 Zillow Real Estate Investment Analyzer

![Build](https://img.shields.io/badge/build-passing-brightgreen)
![Status](https://img.shields.io/badge/status-active-blue)
![License](https://img.shields.io/badge/license-MIT-lightgrey)

A powerful, automated real estate analysis tool that scrapes property data from Zillow, calculates investment metrics like ARV, ideal purchase price, potential profit, and intelligently matches subject properties with comparable (comps) for investors.

---

## 🚀 Features

- ✅ Zillow property scraping using address, zip, or area
- ✅ ARV (After Repair Value) calculation from filtered comps
- ✅ Ideal Purchase Price and Max Offer computation
- ✅ Comp pairing logic (1 subject ➝ 2 unique comps)
- ✅ Intelligent filters: radius, profit margin, repair cost, ARV cap
- ✅ Interactive dashboards or webhook support (n8n compatible)
- ✅ Dynamic lead grading based on deal strength (A+, B, C)

---

<details>
<summary>🧠 <strong>How It Works</strong></summary>

### 📊 Analysis Pipeline

1. **Scrape Zillow Property Details**
2. **Identify Comps within Radius (X miles)**
3. **Filter & Sort by:**
   - Area within ±500 sqft
   - Max ARV
   - Price Range
4. **Calculate:**
   - **ARV**: Avg price of top 3 filtered comps
   - **Profit**: ARV - Repair Cost - Purchase Price
   - **Ideal Purchase Price**: ARV - Repairs - Desired Profit
5. **Return Results via Webhook / Dashboard**

</details>

---
