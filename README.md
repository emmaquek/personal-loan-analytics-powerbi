# Personal Loan Uptake & Credit Stress Signals Dashboard - Power BI

## Project Overview
This project analyses **personal loan acceptance behaviour and early credit stress signals** using customer-level financial data.  
The goal is to demonstrate how **descriptive analytics and visual storytelling** can support decision-making for **financial institutions, regulators, and consumer finance platforms**.

---

## Problem Statement
Financial institutions and regulators need to understand:
- **who accepts personal loan offers**
- **how borrowing behaviour relates to income and credit usage**
- **where potential financial stress may be building up**

However, early stress signals often do not come from defaults alone, but from **patterns of spending relative to income** and **concentration of borrowing among certain customer segments**.

This project addresses the question:
> **How do income, credit card spending, and existing financial relationships influence personal loan acceptance and indicate potential credit stress?**

---

## Dataset
- Publicly available consumer banking dataset (Kaggle)
- Customer-level information including:
  - annual income
  - credit card spending
  - education level
  - personal loan acceptance
  - ownership of CD and securities accounts
  - digital banking usage

### Key Data Transformations
- Credit card spending (monthly, in thousands) was **annualised** and converted to monetary values
- Income values (in thousands) were converted to annual monetary amounts
- A **Credit Card Spend-to-Income ratio** was derived as a proxy for credit stress
- A **High Credit Pressure threshold (30%)** was defined for analytical interpretation

---

## Dashboard Structure

### Page 1 — Borrowing Overview
**Purpose:**  
Provide a high-level view of personal loan acceptance and customer financial context.

**Key Elements:**
- personal loan acceptance rates
- income and spending context
- differences in loan acceptance across education and income bands

**Key Insight:**  
Loan acceptance is concentrated among **higher-income and more financially engaged customers**, with minimal uptake among lower-income segments.

**Rationale:**  
To establish baseline borrowing patterns and identify which customer segments are more likely to accept personal loan offers.

---

### Page 2 — Credit Stress Signals
**Purpose:**  
Explore how **credit usage relative to income** may indicate early financial stress and relate to borrowing behaviour.

**Key Elements:**
- the relationship between income and credit card spending at an individual level
- the distribution of credit spend relative to income
- differences in loan acceptance by ownership of other financial products

**Key Insight:**  
While loan acceptance increases with income, a significant proportion of customers exhibit **elevated credit spend relative to income**, highlighting areas where financial stress may concentrate even outside default events.

**Rationale:**  
To shift from *who borrows* to *how customers are financing their spending*, hence highlighting where credit usage may indicate increased financial strain.

---

## Analytical Rationale
This project deliberately focuses on **descriptive and diagnostic analysis**, rather than predictive modelling.

**Why this approach:**
- Reflects how **regulators** monitor systemic risk and credit concentration
- Aligns with how **fintech platforms** assess user financial health and borrowing behaviour
- Prioritises interpretability and transparency over black-box predictions

Metrics and thresholds are designed to be:
- intuitive to non-technical stakeholders
- defensible in a regulatory or business setting
- suitable for early-stage monitoring rather than ex-post default analysis

---

## Tools & Skills Demonstrated
- Power BI (data modelling, DAX, visual design)
- Data cleaning and unit standardisation
- Ratio-based financial analysis
- Segmentation and comparative analysis
- Analytical storytelling for non-technical audiences
