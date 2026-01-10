#  Namibia's Labour Market & Economic Challenges: A Data-Driven Analysis

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
- **427,093 youth** (ages 15-34) are NEET - Not in education,Not in employment or training
- **55.4% of workers** earn below living wage (N$5,000/month)
- **Inflation at 3.4%(November 2025)** annually - eroding purchasing power
- **52.8% unemployment rate** in worst-hit regions (Kavango)

**My analysis explores:** What are the underlying patterns? Who is most affected? How do different regions compare?

---

##  What I Discovered

### 1️⃣ **Youth Employment Patterns: The 20-24 Transition Gap**

![NEET Progression](images/key_charts/neet_progression.png)

**The Pattern:**
```
Ages 15-19: 16.9% NEET  (Most in education - expected pattern)
Ages 20-24: 47.4% NEET  (Significant transition challenge)
Ages 25-34: 53.4% NEET  (Pattern stabilizes at higher level,No change at this level Ages 20-24 mainly remain NEET)
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
Inflation: 3.4% November inflation 2025 improved from 5.89% average annualy from 2023
Inflation

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

**What This Means for Namibia:**  
Employment is heavily concentrated in sectors with limited wage growth potential and career advancement opportunities. This pattern contributes to the gap between having a job and achieving economic security, and highlights the importance of sectoral diversification and skills development aligned with higher-wage industries.

---

### 6 📈 Economic Context: The GDP-Employment Disconnect

### Why Economic Growth Doesn't Translate to Jobs

![GDP vs Employment](images/key_charts/gdp_employment_disconnect.png)

**The Paradox:** Namibia's economy is dominated by high-productivity sectors that generate wealth but create few jobs, while labour-intensive sectors employ most workers but contribute minimally to GDP.

---

###**GDP Contribution by Sector (2023)**

| Sector | GDP Share(Q4 2023) | Employment Share | Gap |
|--------|-----------|------------------|-----|
| **Mining and Quarrying** | 19.3% | 2.6% | Capital-intensive |
| **Wholesale and Retail Trade** | 11.1% | 10% | Balanced |
| **Manufacturing** | 10.1% | 9.8% | Balanced |
| **Agriculture and Forestry** | 5.7% | **16.1%** | Labour-intensive |
| **Transport and Storage** | 2.9% | 3.3% | Balanced |
| **Electricity and Water** | 2.5% | 0.7% | Capital-intensive |
| **Construction** | 1.2% | 5.2% | Labour-intensive |
Fishing and fish processing on board
---

### **The Key Finding:**

**Mining generates 19.3% of GDP but employs only ~2.6% of workers.**  
**Agriculture employs 16.1% of workers but generates only 5.7% of GDP.**

This 3:1 ratio reveals why:
- GDP can grow while unemployment remains at 36.9%
- Economic growth benefits don't reach most workers
- High-employment sectors offer limited wage growth

---

### **Sector Growth Patterns (Average Annual Growth 2023)**

**Fast-Growing Sectors:**
1. 🔺 **Mining and Quarrying:** 14.573% growth → Employs few workers
2. 🔺 **Wholesale and Retail Trade:** % growth → Employs 10%
3. 🔺 **Manufacturing:** % growth → Employs 9.8%

**Moderate Growth:**
4. **Agriculture and Forestry:** 5.7% growth → Employs 16.1%
5. **Electricity and Water:** 3.3% growth → Employs <2%
6. **Transport and Storage:** 3.1% growth → Employs ~6%

**Slow-Growing Sectors:**
7. **Fishing:** % growth → Employs ~2%
8. **Construction:** % growth → Employs ~8%
9. **Hotels and Restaurants:** % growth → Employs ~5%

---

### **What This Reveals:**

**1. The Capital-Intensive Trap**
- Mining (19.3% GDP, 14.573% growth) is highly productive but creates minimal jobs
- Each mining job generates ~4-6x more GDP than agriculture job
- But mining employs only 2.6% of workforce vs agriculture's 16.1%

**2. The Growth-Employment Gap**
- Fastest-growing sector (Mining: 14.573%) employs fewest people
- Labour-intensive sectors (Agriculture: 5.7%) grow slowest
- Result: Economic growth bypasses most workers

**3. The Agriculture Challenge**
- Employs 16.1% (102,000+ workers)
- Contributes only 5.7% to GDP
- Growing at moderate 5.6% annually
- **Insight:** Low productivity keeps wages suppressed despite high employment

---

### **Policy Implications:**

**The Data Shows:**
Current economic structure creates GDP growth without job creation. To address unemployment:

1. **Boost agricultural productivity** → Raise wages for 16.1% of workforce without shedding jobs
2. **Linkages between sectors** → Mining purchases from local manufacturing/services
3. **Labour-intensive manufacturing** → Target 10.7% growth sector for job expansion
4. **Construction sector support** → Growing slowly (1.5%) despite employing 5.2%

**The Bottom Line:**
Namibia needs growth strategy that prioritizes **job-rich sectors**, not just **GDP-rich sectors**.

---

### **Comparison: High-GDP vs High-Employment Sectors**

```
High GDP, Low Employment (Capital-Intensive):
├─ Mining: 19.3% GDP → 2.6% employment
├─ Manufacturing: 10.1% GDP → 9.8% employment
└─ Electricity: 2.6% GDP → <2% employment

High Employment, Lower GDP (Labour-Intensive):
├─ Agriculture: 16.1% employment → 5.7% GDP
├─ Retail Trade: 12.4% employment → 11.1% GDP (best balance!)
└─ Construction: 8% employment → 1.2% GDP
```

**Best Performer:** Wholesale and Retail Trade (11.1% GDP, 12.4% employment) - nearly balanced!

---

### **Visual Insight: Capital Intensity Ratio**

**Formula:** GDP Share ÷ Employment Share = Capital Intensity

| Sector | Ratio | Interpretation |
|--------|-------|----------------|
| Mining | 19.3% ÷ 2.6% = **7.4** | Extremely capital-intensive |
| Manufacturing | 10.1% ÷ 8% = **1.3** | Moderately capital-intensive |
| Retail Trade | 11.1% ÷ 12.4% = **0.9** | Labour-intensive (balanced) |
| Agriculture | 5.7% ÷ 18.8% = **0.3** | Very labour-intensive |

**Interpretation:**
- Ratio > 2 = Capital-intensive (few jobs per GDP unit)
- Ratio ~ 1 = Balanced (jobs match GDP contribution)
- Ratio < 0.5 = Labour-intensive (many jobs, low GDP)

---

## 🎯 Key Takeaway

**Namibia's unemployment challenge isn't just about jobs - it's about economic structure.**

The economy is optimized for GDP growth through capital-intensive sectors (mining), not employment creation. Even 12% annual growth in mining won't significantly reduce unemployment because it employs so few people.

**Solution requires:** 
- Redirecting growth to labour-intensive sectors (agriculture, manufacturing, services)
- OR improving productivity in existing high-employment sectors
- OR creating stronger linkages so capital-intensive growth benefits labour-intensive sectors

---

## 📊 Data Sources

- **GDP Share:** Namibia StatisticsAgency, GDP by Industry (2023)
- **GDP Growth:** Namibia Statistics Agency, Quarterly GDP Reports (2015-2024 average)
- **Employment Share:** NSA 2023 Labour Force Survey

---

## 🔗 Related Findings

This economic context helps explain:
- **Finding #2:** Why 55.4% earn below living wage (concentration in low-productivity sectors)
- **Finding #4:** Regional disparities (mining concentrated in specific regions)
- **Finding #5:** Sectoral concentration (labour-intensive sectors offer limited wages)

---

**[Previous Finding] ← | → [Next: Implications and Insights]**

---

## Quick Stats Box (Optional - Add to Sidebar/KPI)

```
┌─────────────────────────────────┐
│  GDP-EMPLOYMENT GAP             │
├─────────────────────────────────┤
│  Mining:                        │
│  • 19.3% of GDP                 │
│  • 2.6% of employment           │
│  • 12.0% annual growth          │
│                                 │
│  Agriculture:                   │
│  • 5.7% of GDP                  │
│  • 16.1% of employment          │
│  • 5.6% annual growth           │
│                                 │
│  Capital Intensity Ratio:       │
│  Mining/Agriculture = 16:1      │
└─────────────────────────────────┘
```

---

---
## How I Built This

### The Data Pipeline

```
Excel Files (NSA + Bank of Namibia)
    ↓
Python ETL (pandas + SQLAlchemy)
    ↓
PostgreSQL (15 tables)
    ↓
Power BI (6-page dashboard)
```

### What I Worked With

**Data Sources:**
- Namibia Statistics Agency: 2023 Labour Force Survey
- Namibia Statistics Agency: CPI data (November 2025)
- GDP quarterly data (2015-2024)

**Total Records:** 546,805 employment records analyzed from the NSA Labour Force Survey

**Tools:**
- Python (pandas, SQLAlchemy) - Data cleaning & loading
- PostgreSQL - Data warehouse (15 tables)
- Power BI - Interactive visualization
- Excel - Viewing data,Initial date formatting, and converting to CSVs

---

## The Dashboard

I built a **6-page interactive Power BI dashboard** that lets you explore:

1. **Executive Summary** - Key metrics at a glance
2. **Unemployment Deep Dive** - Regional breakdowns
3. **Youth Crisis Analysis** - NEET progression by age
4. **Income & Inflation** - Purchasing power analysis
5. **Sectoral Analysis** - Employment by industry
6. **Economic Context** - CPI & GDP trends

**[View Screenshots →](powerbi/screenshots/)** | **[Download Dashboard →](powerbi/)**

---

## Implications and Insights

### For Job Seekers:
- **Location matters:** Opportunities concentrated in Khomas
- **Sector matters:** Avoid low-wage traps (Agriculture, Domestic Work)
- **Skills matter:** But only if jobs exist to use them

### For Policy Makers:
- **Target ages 20-24:** Critical intervention window
- **Regional solutions:** Regions like Kavango and Ohangwena needs different approach than Windhoek
- **Wage protection:** Inflation indexing for minimum wage
- **Job creation > training:** Skills don't help if jobs don't exist

### For Businesses:
- **Untapped talent pool:** 427K youth are not working
- **Wage sustainability:** Low wages + inflation = productivity loss
- **Regional expansion:** Underserved markets = opportunity

### For Development Orgs:
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

## For Reproducability

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

## Detailed Documentation

Each folder has its own README with specifics:

- **[data/README.md](data/README.md)** - Data sources, processing steps
- **[scripts/README.md](scripts/README.md)** - Python ETL pipeline explanation
- **[powerbi/README.md](powerbi/README.md)** - Dashboard design & usage
- **[reports/README.md](reports/README.md)** - Full findings document
- **[documentation/README.md](documentation/README.md)** - Technical methodology

---

## Technical Highlights

### Challenge 1: Date Standardization
NSA data had inconsistent formats ("Jan-23", "2023/01", "01-2023")  
**Solution:** Excel preprocessing and Python multi-format parsing  
[Details →](documentation/README.md#challenges)

### Challenge 2: Wide-to-Long Transformation
GDP had quarters as columns - needed long format for analysis  
**Solution:** Custom `unpivot_quarterly()` function in python 
[Details →](documentation/README.md#challenges)

### Challenge 3: PostgreSQL Import Mechanics
COPY command requires files in specific server directory (same folder as postgres application) 
**Solution:** Hybrid approach - COPY for speed, SQLAlchemy for flexibility  
[Details →](documentation/README.md#challenges)

**See all challenges:** [documentation/README.md](documentation/README.md)

---

## Sample Query

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
    
    ROUND(
        (((bracket_min + bracket_max) / 2) * (rate / 100 / 12))::numeric, 
        2
    ) as monthly_loss
FROM income_distribution
CROSS JOIN inflation
WHERE bracket_max IS NOT NULL
ORDER BY bracket_min;
```

**[See queries →](data/processed/README.md#queries)**

---

## Key Statistics Summary

| Metric | Value | Source |
|--------|-------|--------|
| **Unemployment Rate** | 36.9% | NSA 2023 Labour Force Survey |
| **Youth NEET (15-34)** | 427,093 | NSA 2023 |
| **NEET Rate (25-34)** | 53.4% | NSA 2023 |
| **Below Living Wage** | 55.4% (302,210 workers) | NSA 2023 |
| **Inflation (Annual)** | 3.6% | Bank of Namibia 2025 |
| **Regional Gap** | 23 percentage points | Kavango vs //Kharas |


---

## Limitations & Assumptions

**Data Limitations:**
- Cross-sectional (can't track individuals over time)
- Self-reported income (may undercount informal earnings)
- Regional aggregation (can't analyze city-level)
- Informal sector likely undercounted

**Assumptions:**
- Living wage = N$5,000/month (based on cost of living estimates)
- Inflation impacts all income groups proportionally (likely understates impact on poor)
- Employment categories are mutually exclusive

**Impact:** These numbers are likely **floor estimates** or lowerbound estimates - reality may be worse.

---

## 🤝 Connect & Collaborate

I'm passionate about using data to solve real problems.

**PAUL KOITA**  
📧 paulkoitpss@gmail.com  
💼 [LinkedIn]([https://linkedin.com/in/yourprofile](https://www.linkedin.com/in/paul-koita-3821212a2/))  

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
