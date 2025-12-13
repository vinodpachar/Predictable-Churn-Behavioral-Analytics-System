# Data Dictionary — Predictable Churn Project

This folder contains the sample datasets used for the Predictable Churn
behavioral analytics case study. All datasets are provided in CSV format
to ensure portability, transparency, and reproducibility.

---

## 1. Customer Profile Dataset  
**File:** `raw/customer_profile.csv`  
**Grain:** One row per customer

This table captures static customer attributes, contract details,
onboarding outcomes, and final churn status. It is primarily used for
segmentation, cohort analysis, and churn outcome labeling.

### Key Columns

- **customer_id**  
  Unique identifier for each customer.

- **industry**  
  Customer industry segment (e.g., SaaS, Finance, Healthcare).

- **company_size**  
  Customer size category (Small, Mid-Market, Enterprise).

- **region**  
  Geographic region of the customer.

- **plan_type**  
  Subscription tier (Basic, Pro, Enterprise).

- **acquisition_channel**  
  Channel through which the customer was acquired (Sales, Referral, Self-Signup).

- **contract_term_months**  
  Length of the customer contract in months.

- **is_multi_year_contract**  
  Indicates whether the contract spans multiple years.

- **onboarding_completion**  
  Onboarding outcome (Completed, Partial, Failed).

- **cs_touch_model**  
  Customer success engagement model (High-Touch, Tech-Touch, No-Touch).

- **initial_NRR_target**  
  Expected net revenue retention target at onboarding.

- **decision_maker_seniority**  
  Seniority level of the primary decision maker.

- **renewal_status**  
  Renewal outcome at contract end (Renewed, Not Renewed).

- **churn_status**  
  Final churn state (Active, Churned).

- **churn_month**  
  Month in which churn occurred (if applicable).

- **pattern_type**  
  Behavioral cohort assigned to the customer.

- **churn_flag**  
  Binary churn indicator (1 = churned, 0 = retained).

---

## 2. Usage Monthly Dataset  
**File:** `raw/usage_monthly.csv`  
**Grain:** One row per customer per month

This table captures time-series behavioral signals used to detect early
signs of churn risk before renewal failure.

### Key Columns

- **customer_id**  
  Foreign key linking to the customer profile table.

- **month_index**  
  Sequential month number in the customer lifecycle.

- **login_frequency**  
  Frequency of product logins during the month.

- **active_users**  
  Number of active users or seats in the account.

- **feature_usage_rate**  
  Overall feature adoption rate.

- **core_feature_adoption**  
  Usage depth of the product’s core features.

- **support_tickets**  
  Number of support tickets raised in the month.

- **escalations**  
  Count of high-severity support escalations.

- **invoice_paid_on_time**  
  Indicator of timely invoice payment.

- **NPS_score**  
  Customer sentiment score.

- **health_score**  
  Composite customer health indicator.

- **is_churn_month**  
  Flags the month in which churn occurred.

---

## Usage Notes

- The `raw/` folder contains **unmodified source data**.
- Any transformed or derived datasets should be stored in a separate
  processed layer (not committed).
- The datasets are intentionally synthetic but modeled on real SaaS
  customer behavior patterns.
