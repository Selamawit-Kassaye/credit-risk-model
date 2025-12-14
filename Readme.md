# Credit Risk Modeling & Basel II Compliance Summary

## 1. Influence of Basel II on Model Documentation

The **Basel II Accord** necessitates **interpretable and well-documented models** to ensure financial stability:

- **Regulatory Approval:** Supervisors must evaluate the technical assumptions before models are used for capital calculations.
- **Auditability:** Documentation ensures legal or administrative risks do not invalidate risk reductions.
- **Solvency:** Clear interpretability allows banks to justify risk weights assigned to different borrower categories.

## 2. Proxy Variables: Necessity and Business Risks

Since direct "default" events are often rare or unobservable, **proxy variables** (e.g., 90-day delinquencies) are used.

- **Why Necessary:** They increase sample size and allow measurement when direct labels are unavailable.
- **Business Risks:**
  - **Inaccuracy:** Poor proxy correlation leads to incorrect capital reserves.
  - **Opportunity Cost:** Conservative proxies may reject healthy, profitable loans.

## 3. Trade-offs: Simple vs. Complex Models

# Credit Risk Modeling & Basel II Compliance Summary

## 1. Influence of Basel II on Model Documentation

The **Basel II Accord** necessitates **interpretable and well-documented models** to ensure financial stability:

- **Regulatory Approval:** Supervisors must evaluate the technical assumptions before models are used for capital calculations.
- **Auditability:** Documentation ensures legal or administrative risks do not invalidate risk reductions.
- **Solvency:** Clear interpretability allows banks to justify risk weights assigned to different borrower categories.

## 2. Proxy Variables: Necessity and Business Risks

Since direct "default" events are often rare or unobservable, **proxy variables** (e.g., 90-day delinquencies) are used.

- **Why Necessary:** They increase sample size and allow measurement when direct labels are unavailable.
- **Business Risks:**
  - **Inaccuracy:** Poor proxy correlation leads to incorrect capital reserves.
  - **Opportunity Cost:** Conservative proxies may reject healthy, profitable loans.

## 3. Trade-offs: Simple vs. Complex Models

### Trade-offs Between Interpretable and Complex Credit Risk Models

| Feature          | Simple Model (Logistic Regression + WoE)                                                                                     | Complex Model (Gradient Boosting)                                                                                      |
| :--------------- | :--------------------------------------------------------------------------------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------- |
| Interpretability | High — Provides transparent coefficients and clear insights into key risk drivers; widely accepted as an industry benchmark. | Low — Often operates as a “black box,” making transparency and regulatory explainability more challenging.             |
| Performance      | Moderate — Limited in capturing complex non-linear relationships and feature interactions.                                   | High — Excels at modeling non-linear patterns and complex interactions, leading to superior predictive accuracy.       |
| Pre-processing   | Required — Relies on manual binning and WoE transformation to handle non-linearity and monotonicity.                         | Minimal — Naturally handles diverse feature distributions, interactions, and missing values.                           |
| Regulatory Fit   | Strong — Well-suited for regulatory reporting and capital requirement calculations; easy to validate and audit.              | Challenging — Requires additional explainability tools (e.g., SHAP, LIME) to meet regulatory and compliance standards. |
