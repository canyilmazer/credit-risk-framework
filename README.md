# credit-risk-framework
Open, end-to-end credit risk modeling framework covering IRB, IFRS 9, and stress testing. Includes PD, LGD, and EAD modeling with full data preparation, governance, calibration, downturn, and validation structure using Python and Jupyter/Colab
# credit-risk-framework

An open, end-to-end credit risk modeling framework covering IRB, IFRS 9, and stress testing.
The repository includes PD, LGD, and EAD modeling with full coverage of data preparation,
governance, calibration, downturn, and validation, implemented in Python using Jupyter
Notebooks and Google Colab.

---

# Credit Risk Modeling Framework  
### IRB • IFRS 9 • Stress Testing (PD, LGD, EAD)

## 1. Purpose
This repository provides an end-to-end, transparent, and reproducible framework for
credit risk modeling under:
- Basel IRB regulatory capital requirements
- IFRS 9 Expected Credit Loss
- Stress testing and scenario analysis

The framework covers the full lifecycle of **Probability of Default (PD)**,
**Loss Given Default (LGD)**, and **Exposure at Default (EAD)**, including:
- Data preparation and data quality assessment
- Model development and challenger analysis
- Calibration and conservatism
- Downturn and scenario adjustments
- Model testing, governance, and auditability

The objective is methodological clarity, audit readiness, and regulatory alignment
with EBA and ECB expectations, while remaining suitable for research, learning,
and controlled experimentation.

---

## 2. Scope

### Portfolios
- Retail
- Corporate

### Risk parameters
- Probability of Default (application and behavioral concepts)
- Loss Given Default (performing and in-default)
- Exposure at Default and Credit Conversion Factors

### Use cases
- IRB capital estimation
- IFRS 9 impairment calculation (Stage 1, Stage 2, Stage 3)
- Stress testing and scenario analysis

---

## 3. Repository structure

credit-risk-framework/
│
├── notebooks/              # Jupyter notebooks for analysis and modeling
│   ├── 01_data_quality.ipynb
│   ├── 02_sample_creation.ipynb
│   ├── 03_pd_model.ipynb
│   ├── 04_lgd_model.ipynb
│   ├── 05_ead_model.ipynb
│   ├── 06_calibration_moc.ipynb
│   ├── 07_downturn_stress.ipynb
│   └── 08_model_testing.ipynb
│
├── src/                    # Reusable Python modules
│   ├── data_quality.py
│   ├── sampling.py
│   ├── pd_model.py
│   ├── lgd_model.py
│   ├── ead_model.py
│   ├── calibration.py
│   └── utils.py
│
├── docs/                   # Methodology and governance documentation
│   ├── definitions.md
│   ├── segmentation.md
│   ├── rating_framework.md
│   ├── calibration_moc.md
│   ├── downturn.md
│   ├── testing_validation.md
│   └── limitations.md
│
├── configs/                # Configuration files
│   ├── segments.yaml
│   ├── master_scale.yaml
│   ├── scenario_config.yaml
│   └── model_params.yaml
│
├── data/                   # Small synthetic datasets only
│   └── synthetic_sample.csv
│
├── tests/                  # Basic unit tests
│
└── README.md


---

## 4. Methodological coverage

### Data and definitions
- Definition of default and cure
- Delinquency and behavioral indicators
- Exposure, collateral, recovery, and write-off concepts
- Independence period and observation windows
- Discount rate and maximum recovery period
- Treatment of small exposures

### Modeling
- Retail and Corporate segmentation
- Application versus behavioral modeling
- Customer-level versus loan-level assignment
- Variable selection and correlation analysis
- Single-factor and multi-factor analysis
- Challenger models
- Conceptual design and coefficient estimation

### Calibration and conservatism
- PD, LGD, and EAD calibration methodologies
- Margin of Conservatism framework (MoC A, MoC B, MoC C)
- Regulatory LGD
- ELBE and realized LGD calculation

### Downturn and stress
- Downturn identification
- Downturn quantification
- Scenario definition and governance
- Forward-looking PD and LGD adjustments

### Testing and governance
- Discriminatory power and calibration testing
- Stability and score distribution analysis
- Segment-level performance assessment
- Model assumptions and limitations
- Audit trail and reproducibility

---

## 5. Technology
- Python
- Jupyter Notebooks
- Google Colab for execution
- GitHub for version control and collaboration

Notebooks can be opened directly in Google Colab using:


---

## 4. Methodological coverage

### Data and definitions
- Definition of default and cure
- Delinquency and behavioral indicators
- Exposure, collateral, recovery, and write-off concepts
- Independence period and observation windows
- Discount rate and maximum recovery period
- Treatment of small exposures

### Modeling
- Retail and Corporate segmentation
- Application versus behavioral modeling
- Customer-level versus loan-level assignment
- Variable selection and correlation analysis
- Single-factor and multi-factor analysis
- Challenger models
- Conceptual design and coefficient estimation

### Calibration and conservatism
- PD, LGD, and EAD calibration methodologies
- Margin of Conservatism framework (MoC A, MoC B, MoC C)
- Regulatory LGD
- ELBE and realized LGD calculation

### Downturn and stress
- Downturn identification
- Downturn quantification
- Scenario definition and governance
- Forward-looking PD and LGD adjustments

### Testing and governance
- Discriminatory power and calibration testing
- Stability and score distribution analysis
- Segment-level performance assessment
- Model assumptions and limitations
- Audit trail and reproducibility

---

## 5. Technology
- Python
- Jupyter Notebooks
- Google Colab for execution
- GitHub for version control and collaboration

Notebooks can be opened directly in Google Colab using:

---

## 6. Collaboration principles
- All changes are version-controlled using GitHub
- Notebooks are committed with clear and descriptive messages
- Reusable logic is implemented in the `src/` directory
- Methodology and governance are documented in `docs/`
- Only synthetic or non-confidential data is included

---

## 7. Disclaimer
This repository is intended for educational and research purposes only.
It does not represent a production-ready banking model and must not be used
for regulatory reporting without independent validation, formal governance
approval, and institution-specific customization.

---

## 8. Authors
Maintained by practitioners with experience in IRB, IFRS 9, and stress testing
model development, validation, and governance.
