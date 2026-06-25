# 🚀 1000 Company Proposal – Federer ICP (DeepThought)

## 🎯 Objective

Build a verified dataset of **1000 Indian specialty manufacturing companies** that match the Federer ICP.

---

## 📌 ICP Definition

We target companies that are:

- Revenue: ₹50Cr – ₹500Cr  
- Promoter-driven ownership  
- Manufacturing-focused (not trading/distribution)  
- Differentiated / technically strong products  
- Active growth signals (hiring, expansion, exports)

---

## ⚙️ System Overview

Raw Universe (3500–4000 companies)  
↓  
Hard Pre-Filters (rule-based cleanup)  
↓  
Screened Pool (2000–2500 companies)  
↓  
AI ICP Scoring (6-dimension model)  
↓  
First-pass Qualified (1200–1400 companies)  
↓  
Human QA (borderline + low confidence cases)  
↓  
Final Verified Dataset (1000 companies)

---

## 📊 ICP Scoring Framework

Each company is evaluated across 6 dimensions (0–10 each):

- C1: Manufacturing authenticity  
- C2: Revenue fit (₹50Cr–₹500Cr)  
- C3: Differentiation (R&D / IP / specialization)  
- C4: Technical decision-maker presence  
- C5: Market tailwinds / sector strength  
- C6: Growth signals (hiring, expansion, activity)

**Total Score:** /60  
Each score must include evidence + confidence level.

---

## 🌐 Data Sources (Universe Building)

### 1. DSIR Recognized R&D Units
- Strong signal for technical maturity and R&D capability  
- Yield: ~800–1000 companies  
- Limitation: older firms dominate  

---

### 2. Industry Expos
(CPHI India, IMTEX, ELECRAMA, BioAsia, PackEx)  
- Signal: growth intent + market participation  
- Yield: ~600–800 companies  
- Limitation: marketing-budget bias  

---

### 3. BSE SME / NSE Emerge
- Signal: verified financials + revenue visibility  
- Yield: ~400–500 companies  
- Limitation: excludes private MSMEs  

---

### 4. USFDA / EU-GMP / WHO-GMP Facilities
- Signal: export-ready manufacturing + compliance strength  
- Yield: ~300–400 companies  
- Limitation: pharma-heavy skew  

---

### 5. Industry Associations
(ACMA, CII, FICCI, IDMA, ELCINA)  
- Signal: verified industry participation  
- Yield: ~500–600 companies  
- Limitation: dataset overlap  

---

### 6. MCA Database
- Signal: full corporate registry + NIC classification  
- Yield: ~1000–1500 companies  
- Limitation: noisy classification  

---

### 7. LinkedIn Sales Navigator
- Signal: founder / technical leadership mapping  
- Yield: ~300–400 companies  
- Limitation: self-reported data  

---

## 🔧 Processing Pipeline

### Step 1: Universe Creation
Combine all sources into raw dataset (~3500–4000 companies)

---

### Step 2: Pre-Filtering
Remove:
- No website companies  
- Traders / distributors  
- Empty or parked domains  
- Clearly out-of-range revenue firms  

---

### Step 3: Website Enrichment
Scrape:
- Homepage  
- About / Leadership  
- Products  
- Careers  
- News / Press  

---

### Step 4: AI Scoring
- Claude Haiku → first-pass scoring  
- Claude Sonnet → borderline re-evaluation  
- Output structured JSON with evidence  

---

### Step 5: Human QA
- Review low-confidence cases  
- Validate manufacturing authenticity  
- Fix misclassified companies  

---

### Step 6: Final Dataset
Final output = **1000 verified companies**

---

## 📈 Expected Yield Flow

| Stage | Count |
|------|------|
| Raw Universe | 3500–4000 |
| After Filtering | 2000–2500 |
| After AI Scoring | 1200–1400 |
| Final Verified List | **1000 companies** |

---

## 📦 Final Deliverables

- 1000 verified ICP companies  
- 6-dimension scoring with evidence  
- Top 200 priority outreach accounts  
- Source contribution breakdown  
- QA audit log (accept/reject reasoning)  

---

## 🛠 Tools Used

- Python (data processing & scraping logic)  
- Playwright (website scraping)  
- Claude Haiku (bulk scoring)  
- Claude Sonnet (deep evaluation)  
- LinkedIn Sales Navigator  
- MCA / DSIR / Expo datasets  
- Google Sheets / PostgreSQL (tracking & QA)  

---

## 📅 Timeline (30 Days)

- Week 1: Universe building  
- Week 2: Data cleaning + enrichment  
- Week 3: AI scoring + filtering  
- Week 4: Human QA + final dataset  

---

## 📌 Note

This system prioritizes **data quality over volume**, ensuring every company is validated across multiple independent signals before inclusion in the final dataset.
