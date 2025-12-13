# Predictable Churn – A Behavioral Early-Warning Analytics System

This project is a **business-first decision intelligence case study** that demonstrates how SaaS churn can be predicted **months before cancellation** using behavioral signals — without relying on black-box machine learning models.

The system focuses on **interpretability, early warning, and actionability**, making it suitable for Customer Success, Product, and Revenue teams.

---

## Problem Context
Traditional churn analysis is reactive — customers are flagged only when it is too late to intervene.

This project addresses a different question:

**Can churn be anticipated early by observing behavioral deterioration patterns rather than final outcomes?**

---

## Analytical Approach
Customers were analyzed across onboarding quality, usage trends, sentiment signals, and payment behavior.  
Instead of binary churn labels, the system tracks **risk accumulation over time**.

Key behavioral patterns identified:
- Onboarding Failure → Early Churn
- Stable Low Usage → No Churn
- Contract Renewal Despite Low Usage

---

## Leading Indicator Analysis
Behavioral signals tracked **months before churn** include:
- Usage decay curves
- Health score divergence
- NPS trend deterioration
- Support escalation frequency
- Payment risk indicators

---

## Early-Warning Logic
Rather than predicting churn after it happens, the framework focuses on:
- Signal convergence
- Preventable vs non-preventable churn
- Early intervention windows

---

## Key Insights
- **100% of observed churn clustered into two predictable behavioral patterns**
- Health scores diverge significantly **months before churn**, making them strong leading indicators
- Early onboarding failure drives fast churn with minimal recovery window
- Some customers renew despite low usage due to contract structure — exposing false positives in naïve churn models

---

## Business Impact
If deployed in a real SaaS environment, this system would enable teams to:
- Intervene earlier with targeted retention actions
- Prioritize Customer Success effort effectively
- Reduce reactive discounting at renewal
- Align Product, CS, and Finance around shared churn signals

---

## Tools & Methodology
- Microsoft Excel (Pivot tables, cohort logic, trend analysis)
- Structured behavioral rules
- Decision-focused analytical framing

> This project intentionally avoids complex ML to emphasize **interpretability and decision usability**.

---

## Documentation
Detailed analysis, charts, and strategic narratives are available here:  
📄 `docs/Predictable Churn A Behavioral Early-Warning Analytics System.pdf`

---

## Author
**Vinod Pachar**  
Aspiring Data & Business Analyst  
Focused on decision intelligence, behavioral analytics, and strategy-driven insights.
