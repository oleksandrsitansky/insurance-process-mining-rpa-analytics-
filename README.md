# End-to-End Insurance Process Mining & RPA Efficiency Analytics

![Tableau](https://img.shields.io/badge/Tableau-Public-E97627?style=flat&logo=tableau&logoColor=white)
![Domain](https://img.shields.io/badge/Domain-Insurance%20%26%20Claims-blue)
![Methodology](https://img.shields.io/badge/Methodology-Process%20Mining-green)

An end-to-end insurance analytics project focused on claims processing efficiency, Process Mining, Robotic Process Automation (RPA) 
adoption, operational bottlenecks, adjuster performance, and underwriting risk analysis.

The project transforms an insurance claims event log into actionable business insights through Tableau dashboards and supporting 
analytical documentation.

---

## Interactive Dashboard

### Tableau Public

**[View Interactive Dashboard on Tableau Public](https://public.tableau.com/views/End-to-EndInsuranceAnalytics/End-to-EndInsuranceAnalytics?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)**

The dashboard consists of three analytical pages covering executive performance, process efficiency, RPA adoption, and underwriting risk.

---

## Dashboard Overview

### Page 1 — Executive Overview

Provides a high-level overview of the insurance claims portfolio, including:

- Total claims
- Total approved payouts
- Average claim severity
- Payout dynamics over time
- Claims by policy type
- Claims by vehicle brand
- Accident and loss analysis

![Executive Overview](https://github.com/oleksandrsitansky/insurance-process-mining-rpa-analytics-/blob/main/dashboard/preview_p1.png)

---

### Page 2 — Process Mining & RPA Efficiency

Focuses on operational efficiency and claims processing performance:

- End-to-end claim cycle time
- FNOL → Assign bottleneck analysis
- Assign → Decision processing time
- RPA vs Human processing comparison
- Settlement time distribution
- RPA adoption rate
- Adjuster workload and performance

![Process Mining and RPA Efficiency](https://github.com/oleksandrsitansky/insurance-process-mining-rpa-analytics-/blob/main/dashboard/preview_p2.png)

---

### Page 3 — Risk & Underwriting Profile

Analyzes the risk structure of the insurance portfolio:

- Claimant age distribution
- Average claim amount by age group
- Losses by vehicle make and model
- Vehicle manufacturing year analysis
- Accident type dynamics
- Policy type × accident type loss matrix

![Risk and Underwriting Profile](https://github.com/oleksandrsitansky/insurance-process-mining-rpa-analytics-/blob/main/dashboard/preview_p3.png)

---

## Business Objectives

### Cycle Time Reduction

Identify operational bottlenecks across the claims lifecycle and reduce the total time from First Notice of Loss (FNOL) to claim closure.

### RPA Efficiency Assessment

Evaluate the adoption and effectiveness of Robotic Process Automation by comparing automated and human-driven claims processing.

### Underwriting Risk Analysis

Identify high-loss portfolio segments based on:

- Driver age
- Accident type
- Policy type
- Vehicle make
- Vehicle model
- Vehicle manufacturing year

### Adjuster Workload Optimization

Evaluate adjuster performance using:

- Number of processed claims
- Total approved payouts
- Average time to decision

### Executive Monitoring

Provide management with a centralized dashboard for monitoring:

- Claims volume
- Total payouts
- Average claim severity
- Processing time
- RPA adoption
- Portfolio risk

---

## Analytical Approach

### Process Mining & Operational Analysis

The project analyzes the insurance claims event log to identify delays between key process stages.

Key metrics include:

- Average End-to-End Claim Cycle Time
- Individual activity duration
- FNOL → Assign duration
- Assign → Decision duration
- Average and median processing time
- RPA vs Human processing time
- Settlement time distribution

### Financial & Risk Analytics

The analysis evaluates the financial structure of the claims portfolio.

Key analyses include:

- Total approved payouts
- Average claim amount
- Payouts by policy type
- Payouts by vehicle make
- Payouts by vehicle model
- Payouts by manufacturing year
- Accident type analysis
- Policy type × accident type loss matrix
- Claim amount by claimant age

### Workforce Performance

The project evaluates the performance of the Top-10 adjusters using:

- Total processed claims
- Total approved payouts
- Average time to decision

This allows management to compare workload and operational performance across adjusters.

---

## Key Findings

### Primary Process Bottleneck

The **FNOL → Assign** stage takes approximately **15.01 days** on average.

This represents more than **42% of the total claim cycle**, with the overall average cycle time reaching approximately **35.01 days**.

### Decision-Making Speed

Once a claim is assigned to an adjuster, the **Assign → Decision** stage is significantly faster, taking approximately **5.01 days** on average.

### RPA Adoption & Stability

RPA accounts for approximately **35.33%** of processed cases.

The median settlement time for RPA and Human processing is approximately the same at around **35 days**.

However, RPA demonstrates fewer extreme time outliers, indicating greater process consistency and operational stability.

### Adjuster Performance

The Top-10 adjusters process approximately **9–15 cases each**.

Average time-to-decision remains within a relatively narrow range of approximately **19–22 days**.

### High-Loss Vehicle Segments

The largest cumulative payout amounts are associated with high-volume vehicle models, including:

- Ford F-150
- Toyota Camry
- Honda Civic
- Chevrolet Silverado

The highest average claim amounts are observed among selected claimant age groups, particularly the **50–55** and **75–80** brackets.

---

## Business Recommendations

### 1. Automate Claim Assignment

The largest operational opportunity is the FNOL → Assign bottleneck.

Implement automated claim assignment and intelligent routing to reduce waiting time between claim registration and adjuster assignment.

### 2. Refine RPA Decision Rules

Introduce Straight-Through Processing (STP) for low-complexity claims.

Claims below a predefined threshold could be automatically processed when risk and fraud indicators are within acceptable limits.

### 3. Expand RPA Coverage

Increase RPA adoption by extending automation to additional standardized process stages, particularly:

- Set Reserve
- Payment Sent
- Standard Collision claims
- Standard Comprehensive claims

### 4. Improve Underwriting Risk Management

Review pricing, deductibles, and underwriting rules for vehicle segments demonstrating consistently high cumulative losses.

Particular attention should be given to high-loss vehicle models and relevant manufacturing-year cohorts.

---

## Tools & Technologies

| Category | Technology |
|---|---|
| Business Intelligence | Tableau Public |
| Data Analysis | Tableau |
| Analytical Methodology | Process Mining |
| Calculations | Tableau LOD Expressions |
| Data Source | Insurance Claims Event Log |
| Documentation | Markdown / PDF |
| Version Control | Git / GitHub |

---

## Dataset

The project uses a synthetic insurance claims event log containing information about the claims lifecycle, including process activities, 
timestamps, policy characteristics, vehicle information, claimant attributes, payouts, adjusters, and RPA processing.

**Dataset:** `Insurance_data - Insurance_claims_event_log.csv`

---

## Repository Structure

```text
insurance-process-mining-rpa-analytics/
│
├── data/
│   └── Insurance_data - Insurance_claims_event_log.csv
│
├── documentation/
│   ├── (EN) End-to-End Insurance Analytics_ Process Mining, RPA Efficiency & Risk Profile.pdf
│   └── (UA) End-to-End Insurance Analytics_ Process Mining, RPA Efficiency & Risk Profile.pdf
│
├── dashboard/
│   ├── End-to-End Insurance Analytics.twb
│   ├── Interactive_Dashboard.md
│   ├── preview_p1.png
│   ├── preview_p2.png
│   └── preview_p3.png
│
└── README.md

Project Deliverables

The repository contains:

Original insurance claims event log
Interactive Tableau Public dashboard
Tableau workbook source file
Three dashboard preview images
Full analytical documentation in English
Full analytical documentation in Ukrainian
Documentation

Detailed analytical documentation is available in English and Ukrainian in the documentation folder.

The documentation covers:

Strategic Business Objectives
Key Analytical and Technical Tasks
Conclusions
Practical Business Recommendations

The original Tableau workbook is included in the repository:

dashboard/End-to-End Insurance Analytics.twb

The workbook contains the dashboard structure, visualizations, calculated fields, and analytical logic used to produce the final report.

Project Outcome

The project demonstrates an end-to-end analytical workflow:

Raw Event Log → Data Analysis → Process Mining → KPI Calculation → Bottleneck Identification → RPA Analysis → Risk Segmentation → Tableau Dashboard → Business Recommendations

The final solution connects operational process metrics with financial and underwriting insights to support data-driven decision-making in insurance claims management.

---

Author

Oleksandr Sitanskyi

Data Analytics | Business Intelligence | Process Mining