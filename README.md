# Intergenerational Educational Mobility in the Philippines

## 📘 Project Overview
This project analyzes intergenerational educational mobility in the Philippines using microdata from the Philippine Statistics Authority’s Labor Force Survey (LFS). It combines rigorous data cleaning, parent–child pairing, and Bayesian multilevel modeling to explore how parents’ education influences their children’s educational attainment across regions and genders.

---

## ⚙️ Data Preparation
- **Source:** 2016-2024 Labor Force Survey (Public Use File)  
- **Processing Tool:** Python (pandas)  
- **Steps:**
  1. Selected and renamed key household and individual variables.
  2. Filtered valid family members (parents and children) and excluded incomplete or irrelevant records.
  3. Mapped education and occupation codes to meaningful categories.
  4. Constructed parent–child pairs within households.
  5. Generated derived indicators such as schooling years and educational attainment levels.
  6. Exported cleaned datasets for modeling.

---

## 📊 Modeling and Methods
- **Approach:** Bayesian Hierarchical (Multilevel) Regression  
- **Model Goal:** Estimate regional and gender-specific intergenerational educational persistence.
- **Dependent Variable:** Child’s years of schooling  
- **Key Predictor:** Parent’s years of schooling  
- **Controls:** Region-level random effects  

This framework captures both national-level persistence and regional variation in mobility.

---

## 🔍 Key Findings and Insights
### 🧑‍🏫 Father–Son Mobility
- Persistence slopes range from **0.244 (CAR)** to **0.280 (Cagayan Valley)**.  
- Indicates moderate persistence: each additional year of father’s education increases the son’s schooling by about a quarter of a year.  
- Minimal regional differences suggest widespread structural barriers, though lower than older cohort estimates (~0.35), hinting at gradual improvement.

### 👩‍👦 Mother–Son Mobility
- Slopes vary widely (**0.249 NCR → 0.385 Davao**).  
- Stronger and more uneven maternal influence, especially in regions with high poverty or weak school systems (e.g., Bicol, Eastern Visayas, Davao).  
- Suggests maternal education compensates for limited resources in disadvantaged areas.

### 👨‍👧 / 👩‍👧 Daughters’ Mobility
- Generally lower persistence, signaling higher mobility.  
- Father–daughter slopes: **0.08–0.19**, mother–daughter: **0.13–0.24**.  
- Reflects daughters’ higher average schooling and better access to education.  
- Yet, mobility remains constrained in regions with poor educational infrastructure.

---

## 🗺️ Regional Mobility Patterns
When combining average schooling (~11 years) with regional persistence:
| Quadrant | Profile | Regions | Description |
|-----------|----------|----------|--------------|
| **Progressive Accumulation** | High schooling, low persistence | NCR | Equitable access, strong mobility |
| **Progressive Under-Accumulation** | Low schooling, low persistence | BARMM, MIMAROPA | Improving opportunity amid low base |
| **Regressive Accumulation** | High schooling, high persistence | CALABARZON, Central Luzon | High education but strong inheritance |
| **Regressive Under-Accumulation** | Low schooling, high persistence | Bicol, Davao, Eastern Visayas | Structural inequality and low opportunity |

---

## 💡 Policy Implications
- **Targeted regional programs** should address persistent inequality in educational access.
- **Maternal education** investments can significantly enhance mobility in low-resource areas.
- **Gender-sensitive strategies** are needed, as sons remain more tied to parental attainment in most regions.

---

## 🧠 Tools & Technologies
- **Python** for data cleaning (`pandas`, `numpy`)  
- **R / PyMC** for Bayesian hierarchical modeling  
- **Matplotlib / Seaborn** for visualization  

---

## 📈 Conclusion
Intergenerational educational mobility in the Philippines shows **slow but steady progress**. Although educational inheritance remains significant, particularly in disadvantaged regions, younger cohorts exhibit **increasing mobility**—a sign of evolving equity in access and opportunity. Continued investment in **regional and gender-sensitive education policies** is essential to sustain this momentum toward inclusive human capital development.
