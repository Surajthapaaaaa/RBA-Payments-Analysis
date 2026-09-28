# Business Brief: Australian Retail Payments Trends

 ## 1. Background
 Australian payments are shifting away from cash and cheques towards
cards and real-time account-to-account payments through the New
Payments Platform (NPP). For a payments fintech, this changes where
product investment is likely to pay off. This project uses RBA retail
payments statistics to measure which payment types are growing,
which are declining, and what that means for product priorities.


 ## 2. Stakeholder
Head of Product at a Sydney-based payments fintech (hypothetical).

 ## 3. Business Problem
The company must decide where to invest next: card-linked products,
credit products, or account-to-account (NPP) payments.
Which payment types are growing, which are declining, and what does
that mean for product priorities?

 ## 4. Business Questions
a. Which payment types are growing fastest year-on-year?
b. Which are declining, and how quickly?
c. How is the payment mix (share of total value) changing?
d. How seasonal is demand, and does it affect planning?
e. Is debit card growth outpacing credit card growth, and what does
   that imply for which card-linked products to prioritise?

## 5. Success Criteria
- 2-3 clear recommendations, each backed by a number
- Metrics defined in the KPI sheet
- Findings reproducible from the SQL scripts

## 6. Scope
**In scope:** RBA payments tables C1-C6 (cards, ATMs, cheques, NPP).
**Out of scope:** customer-level behaviour, fraud, non-RBA sources.

## 7. Data Sources
-RBA Payments Data (rba.gov.au).
-Tables used: C1/C1.1 (credit and charge cards), C2/C2.1 (debit cards),
-C4/C4.1 (ATMs), C5/C5.1 (cheques), C6/C6.1 (Direct Entry and NPP).
Download date: [date].

 ## 8. Deliverables
KPI definitions, data dictionary, cleaning log, SQL scripts,
dashboard, recommendations.

## 9. Assumptions and Limitations
- Aggregate data only, so no individual customer insight
- Trends show correlation, not causation
- [Add NPP data gap note after you check the data]
