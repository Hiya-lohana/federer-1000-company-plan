📌 1000 Company Proposal (Federer ICP – DeepThought)
Goal

Build a verified list of 1000 companies matching DeepThought’s Federer ICP — Indian specialty manufacturers with ₹50Cr–₹500Cr revenue, promoter-driven structure, differentiated product offerings, technical decision-making presence, and active growth signals — within 30 calendar days.

The focus is precision over volume, ensuring every company is backed by multi-source evidence across 6 ICP dimensions.

Key Constraints
Quality over volume → 1000 verified companies, not scraped dumps
Expected yield: ~30% (from ~3500–4000 sourced universe)
Every company must include 6-dimension ICP scoring with evidence
Sources must be traceable and deduplicated
System Overview (Funnel Design)

Raw Universe (3500–4000 companies)
    ↓
Hard Pre-Filters (rule-based elimination)
    ↓
Screened Pool (2000–2500 companies)
    ↓
AI-Based ICP Scoring (6 criteria evaluation)
    ↓
First-pass Qualified Set (1200–1400 companies)
    ↓
Human QA (borderline + low confidence cases)
    ↓
Final Verified Dataset (1000 companies)

Sourcing the Universe (Week 1)

Objective: Build a high-signal raw universe of 3500–4000 companies

Source 1: DSIR Recognized R&D Units
Maintained by Department of Scientific & Industrial Research
Signals: strong indicator of R&D capability (C3) and technical leadership (C4)
Expected yield: ~800–1000 companies
Limitation: Skewed toward older, established firms
Source 2: Industry Expo Exhibitor Lists

Examples: CPHI India, IMTEX, ELECRAMA, BioAsia, PackEx

Signals: paid participation → growth intent (C6)
Expected yield: ~600–800 companies
Limitation: biased toward marketing-budget-enabled firms
Source 3: BSE SME / NSE Emerge Listings
Signals: verified financial disclosures, revenue visibility
Enables direct mapping to ₹50Cr–₹500Cr band
Expected yield: ~400–500 companies
Limitation: excludes unlisted MSMEs (major ICP segment gap)
Source 4: USFDA / EU-GMP / WHO-GMP Approved Facilities
Signals: compliance-driven manufacturing + export readiness (C1, C5)
Expected yield: ~300–400 companies
Limitation: pharma-heavy distribution bias
Source 5: Industry Association Directories

ACMA, CII, FICCI, IDMA, ELCINA, etc.

Signals: validated industry participation
Expected yield: ~500–600 companies
Limitation: overlap with other datasets
Source 6: MCA (Ministry of Corporate Affairs)
Full registry of Indian companies with NIC classification + directors + capital structure
Signals: foundational corporate verification layer
Expected yield: ~1000–1500 companies
Limitation: noisy NIC coding + outdated classifications
Source 7: LinkedIn Sales Navigator
Reverse mapping via founders / CXOs in manufacturing sectors
Signals: technical leadership presence (C4) + hiring activity
Expected yield: ~300–400 companies
Limitation: self-reported data inaccuracies
Week 1 Output

After deduplication across sources:

👉 ~3500–4000 unique companies
Fields: company name, website (~60%), city, segment tag

Remaining ~40% require automated website discovery via search + enrichment.

Automated ICP Scoring (Week 2–3)
Website Data Extraction

For each company:

Homepage
About / Leadership
Product pages
News / Press
Careers / Jobs
Contact pages

Tech: Playwright-based scraper (~8K tokens per company)

ICP Scoring Model (6 Dimensions)

Each company evaluated on:

C1: Manufacturing authenticity
C2: Revenue fit (₹50Cr–₹500Cr)
C3: Differentiation (R&D / IP / specialization)
C4: Technical decision-maker presence
C5: Market tailwinds / export orientation
C6: Growth signals (hiring, expansion, news)

Output: structured JSON with scores + evidence + confidence flags

Scoring Pipeline
Scrape website data
Claude Haiku → first-pass scoring
Claude Sonnet → borderline re-evaluation
Store structured output in master dataset
Flag low-confidence cases for QA
Hard Pre-Filters (Before AI Layer)
No website available
Parked / empty websites (<2 pages or <500 chars)
Traders / distributors (keyword-based exclusion)
Revenue > ₹500Cr (if identifiable)
Expected Yield Flow

Raw Universe → 3500–4000
After filtering → 2000–2500
After AI scoring → 1200–1400
After QA → 1000 verified companies

Human QA Layer (Week 3–4)
Failure Modes Addressed
C3 inflation (false R&D signals)
C4 misclassification (non-technical founders)
C6 stale growth signals (old news misread as active)
Manufacturing misclassification (service vs production ambiguity)
QA Process
Auto-flag borderline cases (score 40–42 range)
Manual review (~300–400 companies)
Validate:
actual manufacturing proof
leadership credibility
active business signals
Final Deliverables
1000 verified ICP-qualified companies
6-dimension scored dataset with evidence
Top 200 priority accounts (outreach-ready tiering)
Full methodology + source attribution breakdown
QA audit log (accept/reject reasoning)
Tools & Stack
Playwright (scraping layer)
Python (ETL + pipeline logic)
Claude Haiku (bulk scoring)
Claude Sonnet (deep evaluation)
MCA / DSIR / LinkedIn / Expo datasets
Google Sheets / PostgreSQL (storage + QA tracking)
Timeline (30 Days)

Week 1 → Universe creation
Week 2 → Scraping + filtering
Week 3 → AI scoring + refinement
Week 4 → Human QA + final assembly
