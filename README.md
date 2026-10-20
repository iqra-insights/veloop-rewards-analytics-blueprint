# VELOOP Rewards - Product Analytics Blueprint

![Status](https://img.shields.io/badge/data-simulated-orange) ![Deliverables](https://img.shields.io/badge/deliverables-21-blue) ![Events](https://img.shields.io/badge/events-42-informational) ![KPIs](https://img.shields.io/badge/KPIs-54-informational)

**Data Analyst Internship - Task 01: Product Analytics, Data Readiness & Data Management Blueprint**

> **All data used in this project is SIMULATED and fictional. No figure here is an actual VELOOP user, earning, withdrawal, revenue, retention or performance statistic.** Items marked *Proposed* or *To Be Verified* are not claimed to exist in production.

## What this project is

VELOOP Rewards is a rewards and engagement product under development without enough production data for conventional analysis. This project builds the foundation instead: what VELOOP should collect, how to structure it, how to know it is trustworthy, what to measure and what engineering should implement.

## Start here

1. `21_Final_Consolidated_Report.docx` (or `.pdf`) - the complete report with an executive summary.
2. `00_Master_Workbook_All_Sheets.xlsx` - every table in one workbook (22 sheets).
3. Files `01` to `20` - the individual deliverables.

## What is inside

| No. | Deliverable | Files |
|---|---|---|
| 01 | Executive Summary | `.docx` |
| 02 | Product Data Audit | `.docx` |
| 03 | Data Coverage Matrix (31 rows, 14 analytics gaps) | `.xlsx` |
| 04 | User Analytics Specification | `.xlsx`, `.docx` |
| 05 | Earning and Reward Analytics | `.docx` |
| 06 | Wallet and Withdrawal Analytics | `.docx` |
| 07 | Referral and Engagement Analytics | `.docx` |
| 08 | Event Tracking Plan (42 proposed events, `object_action` naming) | `.xlsx` |
| 09 | Data Dictionary (106 fields, 10 entities) | `.xlsx` |
| 10 | Logical Data Model with ER diagram | `.docx` |
| 11 | KPI Catalogue (54 KPIs) | `.xlsx` |
| 12 | Simulated Data Profiling | `.xlsx`, `.docx` |
| 13 | Data Quality Audit (26 issues) and Control Framework (22 rules) | `.xlsx`, `.docx` |
| 14 | Dashboard Blueprint (7 dashboards, 44 visuals, wireframes) | `.xlsx`, `.docx` |
| 15 | Developer Analytics Handoff (14 critical events with acceptance tests) | `.xlsx`, `.docx` |
| 16 | Data Pipeline Proposal | `.docx` |
| 17 | Privacy and Governance Proposal | `.docx` |
| 18 | Analytics Readiness Assessment | `.xlsx`, `.docx` |
| 19 | Assumption and Verification Register (30 assumptions) | `.xlsx`, `.docx` |
| 20 | Implementation Backlog (22 prioritised items) | `.xlsx`, `.docx` |
| 21 | Final Consolidated Report | `.docx`, `.pdf` |
| - | Presentation (7 slides) | `22_Presentation_Task01.pptx` |

## Key findings (simulated data)

- The two supplied workbooks share the same `user_id` values but describe **different people** (0 matching e-mails, names or registration times), so they must never be joined.
- The Users audit sheet contains 8 duplicate rows, 9 rows with a missing value and 1 malformed date.
- The "clean" Users sheet still has state conflicts: for example 72 users with sessions but no login, and 34 users with consent *Pending* but marketing opt-in *Yes*.
- Referral conversion and wallet reconciliation cannot be measured from the supplied data: there is no referrer-to-referred link and no wallet ledger.
- Readiness is scored conservatively: design completeness averages 3.3 / 5, while **verified production readiness is 0 / 5** because no production evidence was supplied.

## Method and integrity rules

- Every product fact carries a status: **Confirmed**, **Proposed** or **To Be Verified**, recorded in the Source and Verification Register.
- Results from simulated data are always worded "In the simulated dataset...".
- No credentials, no invented security rules, and no unnecessary personal data (name and e-mail are excluded from the proposed analytics layer).
- Hard-coded figures in the report were re-checked against the source workbooks.

## Known limitation

The Task 01 workbook that was supplied contained the **Users entity only**. The Task Activity, Rewards, Wallet, Withdrawals, Referrals and Feature Events sheets listed in the brief were not included. Those KPIs are therefore designed and documented but **not tested**. A second, differently labelled workbook was used only as a clearly marked supplementary test bed. The profiling should be re-run when the missing sheets arrive.

## How to read the files

- `.docx` - open in Microsoft Word.
- `.xlsx` - open in Microsoft Excel. Each sheet has a title row and a status legend.
- GitHub does not preview Word and Excel well; download the files or use the PDF report.

## Dashboard prototype

A working user-analytics dashboard built on the SIMULATED Users data: https://veloop-rewards-landing-page-bay.vercel.app/dashboard/

## Related project

Landing page for VELOOP Rewards: https://veloop-rewards-landing-page-bay.vercel.app/ ([repository](https://github.com/iqra-insights/veloop-rewards-landing-page))

## Author

**Iqra Siddiqui** - Data Analyst Intern, VELOOP Rewards (ID: VLRINT202601918)
GitHub: [@iqra-insights](https://github.com/iqra-insights)
