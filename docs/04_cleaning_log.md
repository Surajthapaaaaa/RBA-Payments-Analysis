# Cleaning Log

**Data source:** RBA Payments Data (rba.gov.au)
**Download date:** 28 Sep 2026
**Release date:** 7 Sep 2026
**Cleaned by:** Suraj Thapa
**Tool used for cleaning:** Excel

Raw files are stored untouched in `data/raw/`. All cleaning was done
on copies.

## 1. File Inventory

| # | File | Description | Frequency | First date | Last date | Units |
|---|------|-------------|-----------|------------|-----------|-------|
| 1 | C1.1 | Credit and charge cards, original series | monthly | Jan 1985 | July 2026 | Value: $ Million; Number: '000 |
| 2 | C2.1 | Debit cards, original series | Monthly | May 1994 | July 2026 | Value: $ Million; Number: '000 |
| 3 | C4.1 | ATMs, original series | Monthly | May 1994 | July 2026 | Value: $ Million; Number: '000 |
| 4 | C5.1 | Cheques, original series | Monthly | Jan 2002 | July 2026 | Value: $ Million; Number: '000 |
| 5 | C6.1 | Direct Entry and NPP, original series | Monthly | Jan 2002| July 2026 | Value: $ Million; Number: '000 |

## 2. Cleaning Steps

| # | File | Issue found | Action taken | Rows affected |
|---|------|-------------|--------------|---------------|
| 1 | C1.1 | [ ] | [ ] | [ ] |
| 2 | C1.1 | [ ] | [ ] | [ ] |
| 3 | C2.1 | [ ] | [ ] | [ ] |
| 4 | C4.1 | [ ] | [ ] | [ ] |
| 5 | C5.1 | [ ] | [ ] | [ ] |
| 6 | C6.1 | [ ] | [ ] | [ ] |

Add a row for every change, however small.

## 3. Data Quality Issues and Decisions

### 3.1 Issues and Decisions

| # | Issue | Where (file / series) | Decision | Reason |
|---|-------|-----------------------|----------|--------|
| 1 | [ ] | [ ] | [ ] | [ ] |
| 2 | [ ] | [ ] | [ ] | [ ] |

### 3.2 Coverage by Series

Series in the same file can start and end on different dates.
Blank cells before a series starts are treated as "no data", not zero.

**C1.1**

| Series ID | Metric | Unit | Start | End |
|-----------|--------|------|-------|-----|
| CCCCSTCAV | Value of cash advances | $ million | Jan 1985 | [ ] |
| CCCCSNA | Number of accounts | '000 | [ ] | [ ] |
| CCCCSNAA | Number of active accounts | '000 | [ ] | [ ] |

**C2.1**

| Series ID | Metric | Unit | Start | End |
|-----------|--------|------|-------|-----|
| [ ] | [ ] | [ ] | [ ] | [ ] |

(Repeat for C4.1, C5.1 and C6.1.)

### 3.3 Series Breaks

Dates where the RBA changed how a series is measured. Growth rates
that cross a break may not be like-for-like.

| File | Series ID | Break date | RBA explanation | Treatment in analysis |
|------|-----------|------------|-----------------|-----------------------|
| [ ] | [ ] | [ ] | [ ] | [ ] |

### 3.4 Missing Values and Gaps

| File | Series ID | Period | What is shown in file | Decision |
|------|-----------|--------|-----------------------|----------|
| [ ] | [ ] | [ ] | [ ] | [ ] |

### 3.5 Units and Series Types

Series measured differently are never added or compared directly.

| Type | Examples | Unit in file | Handling |
|------|----------|--------------|----------|
| Value (flow) | [ ] | $ million | [ ] |
| Count of transactions (flow) | [ ] | '000 | [ ] |
| Count at a point in time (stock) | [ ] | '000 | [ ] |

### 3.6 Original vs Seasonally Adjusted

| Decision | Detail |
|----------|--------|
| Series used for growth and share analysis | [original / seasonally adjusted] |
| Reason | [ ] |

## 4. Reshaping (wide to long format)

- Target columns: `date | table | metric | category | unit | value`
- Method: [e.g. Excel Power Query unpivot / manual copy-paste]
- Total rows in final table: [ ]
- Total distinct metrics: [ ]

## 5. Validation Checks

- [ ] Row counts match between clean and raw data (excluding header rows)
- [ ] No duplicate date + metric combinations
- [ ] Spot-checked 5 values against the RBA source file
- [ ] Dates run continuously with no unexpected gaps
- [ ] Units are consistent within each metric

## 6. Output

Cleaned file: `data/clean/rba_payments_tidy.csv`
