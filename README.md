# 📊 Namibia's Labour Market & Economic Challenges: A Data-Driven Analysis

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-15-316192?logo=postgresql)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi)

> **This project explores Namibia’s labour market using official statistics from the Namibia Statistics Agency, analyzing key trends in employment, youth outcomes, income distribution, and regional labour differences.**

<!-- Replace with your actual dashboard screenshot -->
![Dashboard Preview](images/key_charts/dashboard_main.png)

---

## 🎯 Understanding the Challenges

Namibia has **one of the highest unemployment rate in SADC** at **36.9%**.

Beyond this headline statistic:
- 📉 **427,093 youth** (ages 15-34) are NEET - Not in education,Not in employment or training
- 💰 **55.4% of workers** earn below living wage (N$5,000/month)
- 📈 **Inflation at 3.4%(November 2025)** annually - eroding purchasing power
- 🗺️ **52.8% unemployment rate** in worst-hit regions (Kavango)

**My analysis explores:** What are the underlying patterns? Who is most affected? How do different regions compare?

---

## 💡 What I Discovered

### 1️⃣ **Youth Employment Patterns: The 20-24 Transition Gap**

![NEET Progression](images/key_charts/neet_progression.png)

**The Pattern:**
```
Ages 15-19: 16.9% NEET ✅ (Most in education - expected pattern)
Ages 20-24: 47.4% NEET ⚠️ (Significant transition challenge)
Ages 25-34: 53.4% NEET 📊 (Pattern stabilizes at higher level,No change at this level Ages 20-24 mainly remain NEET)
```

**What This Means:**  
Between ages 20-24, a significant transition occurs. School graduates face challenges finding entry-level positions, accessing affordable training, or entering the formal economy. By 25, over half remain outside employment and education - with limited work experience or skills development opportunities.

**This pattern suggests structural challenges in the school-to-work transition.**

---

### 2️⃣ **Income Distribution and the Living Wage Gap**

![Income Distribution](images/key_charts/income_distribution.png)

**The Data:**
- **302,210 workers** (55.4%) earn below N$5,000/month
- Only **2.6%** earn above N$40,000 - indicating income concentration at higher levels

**What This Means:**  
You can work full-time and still be poor. Over half of employed workers can't meet basic needs. The question isn't just "can you find work?" - it's "can you find work that lets you live?"

---

### 3️⃣ **Inflation's Impact on Real Wages**

**The Math:**
```
Worker earning N$1,000/month
Inflation: 3.6% annually

Year 1: N$1,000 → Real value: N$964
Year 2: N$1,000 → Real value: N$929  
Year 3: N$1,000 → Real value: N$897

After 3 years: Lost 10.3% purchasing power
```

**Impact:** 302,210 workers earning below N$5,000 experience a gradual decline in real purchasing power. With fixed nominal wages and rising costs for food, rent, and transport, their economic position becomes increasingly challenging over time.

---

### 4️⃣ **Regional Disparities in Employment Outcomes**

![Regional Map](images/key_charts/regional_unemployment.png)

| Region | Unemployment Rate |
|--------|-------------------|
| **Kavango East** | 52.0% 🔴 |
| **Kavango West** | 52.8% 🔴 |
| **Ohangwena** | 47.2% 🔴 |
| **Khomas** (Capital) | 34.4% 🟡 |
| **//Kharas** | 29.7% 🟢 |

**23 percentage point gap** between best and worst regions.

**What This Means:**  
The data reveals significant regional variation in employment outcomes. National-level policies may not address the distinct economic contexts of different regions. Kavango faces different challenges than Windhoek, suggesting the need for regionally-tailored approaches to employment and economic development.

---

### 5️⃣ **Employment Concentration in Lower-Wage Sectors**

**Employment Concentration:**
- 16.1% → Agriculture (low-wage, seasonal)
- 7.9% → Activities of households as employers; undifferentiated goods- and services-producing activities of households for own use(informal, vulnerable)
- 9.3% → Administrative and support service activities (temporary contracts)

**Nearly 40%** of jobs are low-wage, insecure, with no advancement path.

Meanwhile: Tech, Finance, Professional Services employ **less than 10% combined**.

**What This Means:**  
Employment is heavily concentrated in sectors with limited wage growth potential and career advancement opportunities. This pattern contributes to the gap between having a job and achieving economic security, and highlights the importance of sectoral diversification and skills development aligned with higher-wage industries.

---

## 🛠️ How I Built This

### The Data Pipeline

```
📊 Excel Files (NSA + Bank of Namibia)
    ↓
🐍 Python ETL (pandas + SQLAlchemy)
    ↓
🗄️ PostgreSQL (15 tables)
    ↓
📈 Power BI (6-page dashboard)
```

### What I Worked With

**Data Sources:**
- 📊 Namibia Statistics Agency: 2023 Labour Force Survey
- 📈 Namibia Statistics Agency: CPI data (November 2025)
- 💹 GDP quarterly data (2015-2024)

**Total Records:** 546,805 employment records analyzed from the NSA Labour Force Survey

**Tools:**
- Python (pandas, SQLAlchemy) - Data cleaning & loading
- PostgreSQL - Data warehouse (15 tables)
- Power BI - Interactive visualization
- Excel - Viewing data,Initial date formatting, and converting to CSVs

---

## 📊 The Dashboard

I built a **6-page interactive Power BI dashboard** that lets you explore:

1. **Executive Summary** - Key metrics at a glance
2. **Unemployment Deep Dive** - Regional breakdowns
3. **Youth Crisis Analysis** - NEET progression by age
4. **Income & Inflation** - Purchasing power analysis
5. **Sectoral Analysis** - Employment by industry
6. **Economic Context** - CPI & GDP trends

**[View Screenshots →](powerbi/screenshots/)** | **[Download Dashboard →](powerbi/)**

---

## 🎯 Implications and Insights

### 👥 For Job Seekers:
- **Location matters:** Opportunities concentrated in Khomas
- **Sector matters:** Avoid low-wage traps (Agriculture, Domestic Work)
- **Skills matter:** But only if jobs exist to use them

### 🏛️ For Policy Makers:
- **Target ages 20-24:** Critical intervention window
- **Regional solutions:** Regions like Kavango and Ohangwena needs different approach than Windhoek
- **Wage protection:** Inflation indexing for minimum wage
- **Job creation > training:** Skills don't help if jobs don't exist

### 🏢 For Businesses:
- **Untapped talent pool:** 427K youth are not working
- **Wage sustainability:** Low wages + inflation = productivity loss
- **Regional expansion:** Underserved markets = opportunity

### 🌍 For Development Orgs:
- **Place-based programs:** One-size-fits-all fails
- **Food security:** Food inflation hits poor hardest
- **Youth employment:** Focus on 20-24 transition

---

## 📁 Project Organization

```
NAMIBIA/
├── 📄 README.md                    ← You are here
├── 📂 data/
│   ├── processed/                  ← Clean CSV files ready for analysis
│   └── raw/                        ← Original Excel files from NSA/BoN
├── 📂 documentation/               ← Technical deep-dives
├── 📂 images/key_charts/           ← Dashboard screenshots
├── 📂 powerbi/screenshots/         ← Dashboard page exports
├── 📂 reports/                     ← Full findings write-up
└── 📂 scripts/                     ← Python ETL code
```

**[Explore each folder →](#folder-guides)** Each has its own README with details.

---

## 🚀 Quick Start

Want to reproduce this analysis?

### Option 1: View the Dashboard (Easiest)
1. Go to `powerbi/screenshots/` folder
2. View each dashboard page as PDF/PNG
3. Read the full analysis in `reports/`

### Option 2: Run the Analysis (Intermediate)
1. Download processed data from `data/processed/`
2. Open Power BI file in `powerbi/`
3. Connect to your own PostgreSQL

### Option 3: Rebuild Everything (Advanced)
1. Get raw data from `data/raw/`
2. Run Python scripts in `scripts/`
3. Load to PostgreSQL
4. Open Power BI dashboard

**[Full Setup Guide →](documentation/README.md)**

---

## 📖 Detailed Documentation

Each folder has its own README with specifics:

- **[data/README.md](data/README.md)** - Data sources, processing steps
- **[scripts/README.md](scripts/README.md)** - Python ETL pipeline explanation
- **[powerbi/README.md](powerbi/README.md)** - Dashboard design & usage
- **[reports/README.md](reports/README.md)** - Full findings document
- **[documentation/README.md](documentation/README.md)** - Technical methodology

---

## 🔬 Technical Highlights

### Challenge 1: Date Standardization
NSA data had inconsistent formats ("Jan-23", "2023/01", "01-2023")  
**Solution:** Excel preprocessing → Python multi-format parsing  
[Details →](documentation/README.md#challenges)

### Challenge 2: Wide-to-Long Transformation
GDP had quarters as columns - needed long format for analysis  
**Solution:** Custom `unpivot_quarterly()` function  
[Details →](documentation/README.md#challenges)

### Challenge 3: PostgreSQL Import Mechanics
COPY command requires files in specific server directory (same folder as postgres application) 
**Solution:** Hybrid approach - COPY for speed, SQLAlchemy for flexibility  
[Details →](documentation/README.md#challenges)

**See all challenges:** [documentation/README.md](documentation/README.md)

---

## 📊 Sample Query

Here's how I calculated purchasing power loss:

```sql
-- Show how much each income group loses to inflation
WITH inflation AS (
    SELECT AVG(annual_inflation_rate) as rate
    FROM namibia_cpi
)
SELECT 
    income_bracket,
    total_number as workers,
    -- Wrap the math in parentheses and cast to numeric
    ROUND(
        (((bracket_min + bracket_max) / 2) * (rate / 100 / 12))::numeric, 
        2
    ) as monthly_loss
FROM income_distribution
CROSS JOIN inflation
WHERE bracket_max IS NOT NULL
ORDER BY bracket_min;
```

**[See all 27 queries →](data/processed/README.md#queries)**

---

## 📈 Key Statistics Summary

| Metric | Value | Source |
|--------|-------|--------|
| **Unemployment Rate** | 36.9% | NSA 2023 Labour Force Survey |
| **Youth NEET (15-34)** | 427,093 | NSA 2023 |
| **NEET Rate (25-34)** | 53.4% | NSA 2023 |
| **Below Living Wage** | 55.4% (302,210 workers) | NSA 2023 |
| **Inflation (Annual)** | 3.6% | Bank of Namibia 2025 |
| **Regional Gap** | 23 percentage points | Kavango vs //Kharas |


---

## ⚠️ Limitations & Assumptions

**Data Limitations:**
- Cross-sectional (can't track individuals over time)
- Self-reported income (may undercount informal earnings)
- Regional aggregation (can't analyze city-level)
- Informal sector likely undercounted

**Assumptions:**
- Living wage = N$5,000/month (based on cost of living estimates)
- Inflation impacts all income groups proportionally (likely understates impact on poor)
- Employment categories are mutually exclusive

**Impact:** These numbers are likely **floor estimates** - reality may be worse.

---

## 🤝 Connect & Collaborate

I'm passionate about using data to solve real problems.

**PAUL KOITA**  
📧 paulkoitpss@gmail.com  
💼 [LinkedIn](https://linkedin.com/in/yourprofile)  

**Open to:**
- Data Analyst / Economic Research roles
- Collaboration on Southern Africa development projects
- Speaking about data-driven policy
- Consulting on labour market analysis

---

## 🙏 Acknowledgments

- **Namibia Statistics Agency** - Open, accessible data
- **Bank of Namibia** - Economic indicators
- **The 427,093 NEET youth** - Understanding their employment patterns
- **The 302,210 workers earning < N$5,000** - Illuminating income distribution patterns

---

## 📄 License

This project is open source under the MIT License.

**Citation:**
```
Paul Koita. (2025). Namibia's Labour Market & Economic Challenges: A Data-Driven Analysis. 
GitHub: https://github.com/yourusername/namibia-labour-analysis
Data: Namibia Statistics Agency (2023-2025), Bank of Namibia (2025)
```

---

## ⭐ If This Helped You

If you found this analysis valuable:
- ⭐ **Star this repository** (helps others discover it)
- 🔄 **Share on LinkedIn** (spread awareness)
- 💬 **Open an issue** if you find insights I missed
- 🤝 **Contribute** if you have additional data

---

**Built with:** Python • PostgreSQL • Power BI • Excel 

**Tags:** `unemployment-analysis` `namibia` `sadc` `youth-employment` `neet-crisis` `data-analysis` `postgresql` `power-bi` `economic-research` `southern-africa`
