# Hi, I'm Steve Wang

I'm a USC M.S. Business Analytics student building toward **Risk Analytics, Quantitative Research, and Data/ML Engineering** roles.

My work sits at the intersection of **financial data engineering, machine learning, portfolio construction, and decision-focused analytics**. I like projects where raw, messy data has to become a reliable research pipeline, a model input, and finally a decision framework.

---

## Current Focus

- **Quantitative equity research**: cross-sectional factors, factor timing, backtesting, and portfolio allocation
- **Risk-aware portfolio construction**: mean-variance optimization, Black-Litterman-style views, covariance estimation, and transaction-cost-aware evaluation
- **Data engineering for research workflows**: WRDS/CRSP/Compustat ingestion, DuckDB storage, reproducible panel construction, and modular pipeline design
- **Applied machine learning**: predictive modeling, feature engineering, model diagnostics, and out-of-sample validation

---

## Featured Research Project

### Cross-Sectional Multi-Factor Equity Strategy *(Private Research Repo)*

A modular quantitative equity research pipeline for transforming raw market and accounting data into factor returns, ML-based views, and portfolio allocation inputs.

**Research framing:**

> How can noisy ML-based factor timing signals be converted into uncertainty-aware portfolio views and used inside a Bayesian allocation framework?

**Current pipeline:**

```text
WRDS / CRSP / Compustat / FF data
        ↓
cleaned stock-month and stock-day panels
        ↓
characteristic construction and factor sleeves
        ↓
integrated long factor panel with realized, rolling, holding, and target features
        ↓
ML / z-score factor timing signals
        ↓
Black-Litterman-style P, Q, Ω view-system prototypes
        ↓
structured covariance, posterior expected returns, and allocation research
        ↓
strategy backtesting and diagnostics
```

**Implemented / in progress:**

- WRDS raw data download and local storage workflow
- CRSP/Compustat cleaning, CCM merge, and characteristic-panel construction
- 2x3 factor holding and factor return construction
- Enriched stock-level holding panel with weights, weight changes, bid-ask spread, and transaction-cost fields
- Integrated long factor panel with realized returns, holding features, rolling features, and ML targets
- Daily CRSP/FF5 preparation, daily characteristic construction, and month-end signal snapshots with explicit `SIGNAL_MONTH` / `TARGET_MONTH` timing
- Long-only mean-variance strategy baseline across long-short factor sleeves
- Black-Litterman-style view construction prototypes: View Matrix `P`, View Vector `Q`, residual-based View Uncertainty `Ω`, structured covariance, implied prior returns, and posterior expected-return handoff

**Current priorities:**

- Validate timing, delisting returns, and transaction-cost edge cases
- Strengthen portfolio construction beyond historical-mean max Sharpe
- Tune covariance and view-uncertainty assumptions
- Expand factor coverage before relying on category-relative factor views

**Tech stack:** Python, Pandas, NumPy, Scikit-learn, SciPy, DuckDB, WRDS, CRSP, Compustat, Fama-French data, Jupyter, Git

---

## Public Project

### [Personal Finance Analytics System](https://github.com/dtstevee/personal-finance-analytics)

A modular end-to-end analytics system for multi-source credit-card transaction data. It ingests Amex and Discover transactions, normalizes heterogeneous schemas, deduplicates repeated uploads, stores persistent transaction history, and generates monthly/yearly spending reports through a Streamlit dashboard.

**Tech stack:** Python, Pandas, Streamlit, Scikit-learn

---

## Technical Toolkit

**Languages:** Python, SQL  
**Data & Research:** Pandas, NumPy, DuckDB, WRDS, Jupyter  
**Machine Learning:** Scikit-learn, regression/classification, feature engineering, model validation  
**Quant & Risk:** factor research, portfolio theory, Black-Litterman, mean-variance optimization, covariance estimation, backtesting, transaction-cost modeling  
**Visualization & Apps:** Matplotlib, Seaborn, Streamlit  
**Workflow:** Git, GitHub, VS Code, modular research architecture

---

## What I'm Building Toward

I'm currently focused on projects that connect **data infrastructure → model design → risk-aware decision-making**. My near-term goal is to develop stronger research and engineering experience for roles in:

- Risk Analytics / Model Risk / Market Risk
- Quantitative Research / Quantitative Strategy
- Data Analytics / Business Intelligence
- Applied Machine Learning / Data Engineering

---

## Contact

- **LinkedIn:** [linkedin.com/in/dtsteve](https://www.linkedin.com/in/dtsteve)
- **Email:** he.wang2002@gmail.com
