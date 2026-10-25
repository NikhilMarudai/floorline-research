# Expansion market sizing from Census counts (CBP 2023, SUSB 2022)
Generated: 2026-10-25 · Agent: research-expansion · Status: complete

## Summary
- The 19 listed category codes outside furniture hold 169,555 US establishments with fewer than 20 employees (CBP 2023). At $200, $300 or $450 per store per month that is $406.9M, $610.4M or $915.6M ARR if every one subscribed [F-expansion-23].
- Dropping the four contrast codes (new car dealers, hardware, outdoor power equipment, florists) leaves 134,440 small stores in the 15 negotiated-price codes: $322.7M / $484.0M / $726.0M ARR at $200 / $300 / $450 [F-expansion-24].
- The top 6 negotiated-price codes (used cars, jewelry, sporting goods, used merchandise, electronics, other home furnishings) hold 97,839 small stores, 4.9 times the 20,098 small furniture stores: $234.8M / $352.2M / $528.3M ARR [F-expansion-26].
- Used car dealers are the largest single pool: 23,872 small lots (94.9% of 25,147), and their 22,316 small firms average $2.91M in receipts, about twice the $1.41M of small furniture firms [F-expansion-01].
- Jewelry is the closest analog to furniture: 19,396 small stores (97.5% of all), small-firm average receipts of $1.26M against $1.41M for furniture, and 13,245 small firms [F-expansion-02].
- No clean code exists for pawn shops (in 522298 with other non-bank lenders), hot tub and pool stores (in the 453998 catch-all) or bicycle shops (inside 451110 sporting goods). Mattress stores sit inside furniture, 442110 [F-expansion-03, F-expansion-20, F-expansion-21, F-expansion-22].

## Findings
### F-expansion-23 — 169,555 small stores across all 19 listed codes
- **Value:** 169,555 establishments under 20 employees (2023). ARR $406.9M at $200/mo, $610.4M at $300/mo, $915.6M at $450/mo. Counting only establishments owned by firms under 20 employees (SUSB 2022), the figure is 136,220.
- **Source:** [County Business Patterns 2023, cbp23us.txt](https://www2.census.gov/programs-surveys/cbp/datasets/2023/cbp23us.zip) — US Census Bureau, file dated 2025-05-29; cross-check from [SUSB 2022 us_state_6digitnaics_2022.txt](https://www2.census.gov/programs-surveys/susb/tables/2022/us_state_6digitnaics_2022.txt)
- **Confidence:** high for the counts; the ARR figures are arithmetic at 100% adoption, not a forecast.
- **Use:** pitch | submission-research

### F-expansion-24 — 134,440 small stores in the 15 negotiated-price codes
- **Value:** 134,440 establishments under 20 employees (2023); ARR $322.7M / $484.0M / $726.0M at $200 / $300 / $450. Firm-owned cross-check: 108,275.
- **Source:** CBP 2023 cbp23us.txt (as above)
- **Confidence:** high for the counts; which codes count as "negotiated" is our judgment, not Census's.
- **Use:** pitch | submission-research

### F-expansion-25 — Top 6 of all 19 codes: 102,507 small stores
- **Value:** 441120, 448310, 451110, 453310, 444130 (hardware, a contrast code), 443142: 102,507 establishments; ARR $246.0M / $369.0M / $553.5M.
- **Source:** CBP 2023 cbp23us.txt
- **Confidence:** high
- **Use:** pitch

### F-expansion-26 — Top 6 core codes: 97,839 small stores
- **Value:** 441120 used cars, 448310 jewelry, 451110 sporting goods, 453310 used merchandise, 443142 electronics, 442299 other home furnishings: 97,839 establishments under 20 employees (2023); ARR $234.8M / $352.2M / $528.3M. Firm-owned cross-check: 77,474.
- **Source:** CBP 2023 cbp23us.txt; SUSB 2022 file (cross-check)
- **Confidence:** high
- **Use:** pitch | video-opener

### F-expansion-01 — Used car dealers (441120) are the largest negotiated pool
- **Value:** 25,147 establishments, 94.9% under 20 (23,872), as of 2023; 23,577 firms in 2022, of which 22,316 had under 20 employees and averaged $2.91M in receipts. Total receipts $166.1B (2022).
- **Source:** CBP 2023 cbp23us.txt naics=441120; SUSB 2022 NAICS=441120
- **Confidence:** high
- **Use:** pitch | submission-research

### F-expansion-02 — Jewelry stores (448310) are the closest furniture analog
- **Value:** 19,897 establishments, 97.5% under 20 (19,396), as of 2023; 13,668 firms, 13,245 under 20 averaging $1.26M in receipts (2022); total receipts $41.9B.
- **Source:** CBP 2023 naics=448310; SUSB 2022 NAICS=448310
- **Confidence:** high
- **Use:** pitch

### F-expansion-03 — Sporting goods (451110) includes bicycle shops; they cannot be split out
- **Value:** 20,373 establishments, 85.8% under 20 (17,481), as of 2023; 14,243 small firms averaging $1.06M (2022). The 2017 NAICS index puts "Bicycle (except motorized) shops" in 451110, used bicycle shops in 453310 and motorized bicycle shops in 441228. Neither file publishes a bicycle-only count.
- **Source:** CBP 2023 naics=451110; SUSB 2022; [2017 NAICS Index File](https://www.census.gov/naics/2017NAICS/2017_NAICS_Index_File.xlsx)
- **Confidence:** high for the count. Bicycle shops are not found as a separate figure.
- **Use:** submission-research

### F-expansion-20 — Furniture baseline (442110) includes mattress stores
- **Value:** 21,964 establishments, 91.5% under 20 (20,098); 12,708 firms; 11,441 small firms averaging $1.41M; total receipts $76.4B, an average of $6.01M across all firms. The 2017 NAICS index lists "Mattress stores (including waterbeds)" under 442110, so mattress stores are already in the baseline. This run reproduces the stated baseline and clarifies that the $1.41M average is for firms under 20 employees, not for all 12,708 firms.
- **Source:** CBP 2023 naics=442110; SUSB 2022 NAICS=442110; 2017 NAICS Index File
- **Confidence:** high
- **Use:** submission-research

### F-expansion-21 — Hot tub and pool supply stores have no clean code
- **Value:** The 2017 NAICS index lists "Hot tub stores" and "Swimming pool supply stores" under 453998, All Other Miscellaneous Store Retailers (except Tobacco), a catch-all code. It holds 24,598 establishments (23,102 under 20) as of 2023, and the hot tub and pool share is not found. Kept as a reference row and left out of all totals.
- **Source:** CBP 2023 naics=453998; 2017 NAICS Index File
- **Confidence:** low as a proxy for hot tub stores
- **Use:** submission-research

### F-expansion-22 — Most pawn shops sit outside used merchandise (453310)
- **Value:** The 2017 NAICS index puts "Pawnshops" in 522298, All Other Nondepository Credit Intermediation: 9,373 establishments (8,999 under 20) as of 2023, mixed with other non-bank lenders. 453310 (antiques, consignment, thrift) therefore leaves out most pawn shops. The pawn-only count is not found. 522298 is left out of all totals.
- **Source:** CBP 2023 naics=522298; 2017 NAICS Index File
- **Confidence:** low as a proxy for pawn shops
- **Use:** submission-research

The per-category figures for every other code are F-expansion-04 to F-expansion-19 in the JSON sidecar. Their IDs follow the rank order in table (b).

## Tables

**Code mapping.** Both files use 2017 NAICS, and no 2022 crosswalk was needed. The SUSB 2022 6-digit file still uses 442110, 448310, 453310 and so on, and its furniture row (12,708 firms) matches the baseline. CBP figures are for all legal forms (lfo "-"). "Under 20" in CBP means establishments in the size classes <5, 5–9 and 10–19 employees, which includes establishments with no March employees. In SUSB, "under 20" is the enterprise size class "05: <20" (ENTRSIZE 33). SUSB receipts are in $1,000 in the file and are converted to dollars here. The noise flag is G (low) for every row except 443142 electronics, which is H (moderate noise, 2–5%).

**(a) Census figures by category** (CBP 2023 for establishments; SUSB 2022 for firms and receipts)

| Category | NAICS used | US establishments | % under 20 employees (count) | Firms: total / under 20 | Avg receipts, firms under 20 | Total receipts (all firms) |
|---|---|---|---|---|---|---|
| Used car dealers | 441120 | 25,147 | 94.9% (23,872) | 23,577 / 22,316 | $2.91M | $166.1B |
| New car dealers (contrast, mostly franchised) | 441110 | 21,910 | 28.0% (6,131) | 16,596 / 5,209 | $6.52M | $1,179.9B |
| Recreational vehicle dealers | 441210 | 2,972 | 68.3% (2,030) | 2,153 / 1,638 | $3.54M | $43.3B |
| Boat dealers | 441222 | 4,246 | 89.2% (3,787) | 3,549 / 3,141 | $3.09M | $24.2B |
| Motorcycle, ATV and all other motor vehicle dealers | 441228 | 6,688 | 82.3% (5,506) | 5,965 / 4,834 | $3.23M | $41.7B |
| Jewelry stores | 448310 | 19,897 | 97.5% (19,396) | 13,668 / 13,245 | $1.26M | $41.9B |
| Floor covering stores | 442210 | 9,723 | 93.3% (9,073) | 7,846 / 7,222 | $1.78M | $29.5B |
| Window treatment stores | 442291 | 2,209 | 98.1% (2,167) | 1,901 / 1,837 | $0.98M | $2.8B |
| All other home furnishings stores | 442299 | 11,046 | 82.8% (9,143) | 6,987 / 6,617 | $0.84M | $30.4B |
| Household appliance stores | 443141 | 5,433 | 89.8% (4,881) | 3,931 / 3,445 | $1.53M | $21.2B |
| Electronics stores (receipts flag H) | 443142 | 13,615 | 87.9% (11,972) | 8,660 / 8,058 | $0.95M | $67.2B |
| Musical instrument and supplies stores | 451140 | 3,230 | 86.2% (2,784) | 2,374 / 2,198 | $0.82M | $5.2B |
| Used merchandise stores (antiques, consignment, thrift; excludes most pawn) | 453310 | 19,466 | 82.1% (15,975) | 12,941 / 11,443 | $0.63M | $19.9B |
| Hardware stores (contrast) | 444130 | 15,694 | 88.0% (13,811) | 9,294 / 7,641 | $1.33M | $36.7B |
| Outdoor power equipment stores (contrast) | 444210 | 3,878 | 93.1% (3,609) | 3,849 / 3,509 | $1.67M | $13.4B |
| Sporting goods stores (bicycle shops inside, not separable) | 451110 | 20,373 | 85.8% (17,481) | 15,425 / 14,243 | $1.06M | $62.8B |
| Manufactured (mobile) home dealers | 453930 | 1,746 | 97.9% (1,709) | 1,151 / 1,065 | $3.26M | $9.9B |
| Florists (contrast) | 453110 | 11,834 | 97.7% (11,564) | 11,569 / 11,209 | $0.45M | $6.4B |
| Art dealers | 453920 | 4,729 | 98.6% (4,664) | 4,565 / 4,474 | $1.19M | $10.1B |
| *Furniture incl. mattress stores (baseline)* | 442110 | 21,964 | 91.5% (20,098) | 12,708 / 11,441 | $1.41M | $76.4B |
| *Other misc. retail, holds hot tub/pool (reference, catch-all)* | 453998 | 24,598 | 93.9% (23,102) | 18,291 / 16,856 | $1.09M | $39.9B |
| *Other non-bank credit, holds pawnshops (reference, mixed)* | 522298 | 9,373 | 96.0% (8,999) | 4,700 / 4,325 | $0.99M | $61.3B |

**(b) Addressable small stores and ARR, sorted descending.** Addressable stores are CBP 2023 establishments under 20 employees. ARR = stores × price × 12 at 100% adoption. The SUSB column counts establishments owned by firms under 20 employees (2022). It strips out small branches of chains and is the closer proxy for independent stores.

| Rank | Category (NAICS) | Addressable stores (CBP est. <20) | SUSB est. of firms <20 | ARR at $200 | ARR at $300 | ARR at $450 |
|---|---|---|---|---|---|---|
| 1 | Used car dealers (441120) | 23,872 | 22,625 | $57.3M | $85.9M | $128.9M |
| 2 | Jewelry stores (448310) | 19,396 | 13,533 | $46.6M | $69.8M | $104.7M |
| 3 | Sporting goods incl. bicycle (451110) | 17,481 | 14,666 | $42.0M | $62.9M | $94.4M |
| 4 | Used merchandise (453310) | 15,975 | 11,569 | $38.3M | $57.5M | $86.3M |
| 5 | Hardware, contrast (444130) | 13,811 | 7,771 | $33.1M | $49.7M | $74.6M |
| 6 | Electronics (443142) | 11,972 | 8,333 | $28.7M | $43.1M | $64.6M |
| 7 | Florists, contrast (453110) | 11,564 | 11,342 | $27.8M | $41.6M | $62.4M |
| 8 | All other home furnishings (442299) | 9,143 | 6,748 | $21.9M | $32.9M | $49.4M |
| 9 | Floor covering (442210) | 9,073 | 7,527 | $21.8M | $32.7M | $49.0M |
| 10 | New car dealers, contrast (441110) | 6,131 | 5,239 | $14.7M | $22.1M | $33.1M |
| 11 | Motorcycle, ATV and other motor vehicle dealers (441228) | 5,506 | 4,918 | $13.2M | $19.8M | $29.7M |
| 12 | Household appliance (443141) | 4,881 | 3,617 | $11.7M | $17.6M | $26.4M |
| 13 | Art dealers (453920) | 4,664 | 4,596 | $11.2M | $16.8M | $25.2M |
| 14 | Boat dealers (441222) | 3,787 | 3,210 | $9.1M | $13.6M | $20.4M |
| 15 | Outdoor power equipment, contrast (444210) | 3,609 | 3,593 | $8.7M | $13.0M | $19.5M |
| 16 | Musical instrument and supplies (451140) | 2,784 | 2,285 | $6.7M | $10.0M | $15.0M |
| 17 | Window treatment (442291) | 2,167 | 1,864 | $5.2M | $7.8M | $11.7M |
| 18 | Recreational vehicle dealers (441210) | 2,030 | 1,661 | $4.9M | $7.3M | $11.0M |
| 19 | Manufactured (mobile) home dealers (453930) | 1,709 | 1,123 | $4.1M | $6.2M | $9.2M |
| ref | Furniture incl. mattress (442110) | 20,098 | 11,954 | $48.2M | $72.4M | $108.5M |
| ref | Other misc. retail, hot tub/pool inside (453998) | 23,102 | 17,934 | $55.4M | $83.2M | $124.8M |
| ref | Other non-bank credit, pawnshops inside (522298) | 8,999 | 4,643 | $21.6M | $32.4M | $48.6M |

**(c) Totals** (reference rows 442110, 453998 and 522298 excluded unless stated)

| Set | Codes | Addressable stores | SUSB est. of firms <20 | ARR at $200 | ARR at $300 | ARR at $450 |
|---|---|---|---|---|---|---|
| All 19 listed codes (core + contrast) | 19 | 169,555 | 136,220 | $406.9M | $610.4M | $915.6M |
| Core negotiated codes only (contrast excluded) | 15 | 134,440 | 108,275 | $322.7M | $484.0M | $726.0M |
| Top 6 of all 19 (441120, 448310, 451110, 453310, 444130, 443142) | 6 | 102,507 | 78,497 | $246.0M | $369.0M | $553.5M |
| Top 6 core (441120, 448310, 451110, 453310, 443142, 442299) | 6 | 97,839 | 77,474 | $234.8M | $352.2M | $528.3M |
| Furniture 442110 alone, for scale | 1 | 20,098 | 11,954 | $48.2M | $72.4M | $108.5M |
| All 19 + furniture | 20 | 189,653 | 148,174 | $455.2M | $682.8M | $1,024.1M |

## Gaps and unverified
- The ARR figures assume every small store subscribes. They are a ceiling on the market, not a revenue forecast, and no adoption rate was applied.
- Which codes are "negotiated or item-priced" and which are "contrast" is our judgment, not a Census field. Census measures no negotiation intensity.
- CBP "under 20 employees" counts single establishments, so it includes small branches of chains (for example mall jewelry chains and franchised new car points). The SUSB "establishments of firms under 20" column is the independent-store proxy. It is from 2022, a year earlier than CBP.
- Not found as separate counts: bicycle shops (inside 451110), hot tub and pool supply stores (inside 453998), pawn shops (inside 522298), mattress-only stores (inside 442110), piano stores (inside 451140). Antique and consignment shops are inside 453310 alongside thrift stores, and charity thrift operations make that code less of a fit.
- Nonemployer businesses (no payroll) are in neither file. Many one-person used car lots, art dealers and antique sellers are therefore missing.
- SUSB receipts for 443142 electronics carry noise flag H (moderate, 2–5%). All other receipts are flagged G.

## Sources
1. County Business Patterns 2023, US national file cbp23us.txt (in cbp23us.zip), US Census Bureau, file dated 2025-05-29. https://www2.census.gov/programs-surveys/cbp/datasets/2023/cbp23us.zip
2. Statistics of US Businesses 2022, US and state by 6-digit NAICS, us_state_6digitnaics_2022.txt, US Census Bureau. https://www2.census.gov/programs-surveys/susb/tables/2022/us_state_6digitnaics_2022.txt
3. 2017 NAICS Index File, US Census Bureau. https://www.census.gov/naics/2017NAICS/2017_NAICS_Index_File.xlsx

Reproduce: scripts and extracted rows are in `11-work/` (`scripts/build.py` → `rows.json`, `scripts/tables.py`, `scripts/sidecar.py`; raw downloads in `11-work/dl/`).
