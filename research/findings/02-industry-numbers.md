# Industry numbers — independent furniture retail (US, California bonus)
Generated: 2026-10-24 · Agent: research-industry · Status: partial

Partial because: no furniture-specific aged-inventory benchmark, no published commission-rate survey, no per-stop in-house delivery cost, and no recent (post-2013) haggling survey were found before the session's web-search budget ran out. Everything below has a URL; government files were downloaded and parsed directly (Census CBP 2023, SUSB 2022, ARTS 2022, MRTS via FRED) and 10-Ks were read from EDGAR.

## Summary
- The market is small-firm by structure: 21,964 US furniture-store establishments, 91.5% with under 20 employees; 90% of the 12,708 furniture-store firms have under 20 employees and average $1.4M revenue; California has 2,203 stores, 94% under 20 employees [F-industry-01, 02, 03, 04].
- US furniture stores (NAICS 4421) sold $68.9B in 2024 and furniture + home furnishings stores $125.0B; firms under 500 employees take 45% of furniture-store receipts [F-industry-05, 03].
- Gross margin is about half the ticket (Census ARTS 51.0% in 2022; Furniture Today median 50% in 2019), so every point of discount removes ~2% of gross profit; the median store turns stock ~3 times a year, roughly 120 days of inventory [F-industry-07, 08, 10].
- Sales staff are mostly paid on revenue: nearly half commission-only (2016), typical rates 4–8%, a quoted plan at 6%; a 10% discount cuts the rep's pay 10% but the store's gross profit 20% [F-industry-13, 14, 16].
- Customers negotiate and win: 71% of furniture hagglers got a discount (2009), average furniture saving ~$300 (2013); 60% of 2025 furniture buyers felt they overpaid; ~40% of big-item buyers say they would defect without free shipping [F-industry-17, 18, 19, 20].
- Delivery is a real cost that fees do not cover even at scale: Havertys' delivery fees recovered 79% of its $37.1M delivery cost in 2024 (5.1% of sales); owners of microbusinesses report a 60-hour median week, 62% over 50 hours [F-industry-22, 27].

## Findings

### F-industry-01 — 21,964 US furniture-store establishments; 77% have under 10 employees, 91.5% under 20
- **Value:** 21,964 establishments, 194,508 employees, $9.82B annual payroll (NAICS 442110 Furniture Stores, data as of March 2023). Size classes: <5 employees 11,483; 5–9 5,523; 10–19 3,092; 20–49 1,537; 50–99 206; 100–249 71; 250–499 40; 500–999 9; 1,000+ 3. Under 10: 17,006 (77.4%); under 20: 20,098 (91.5%).
- **Source:** [County Business Patterns 2023, US file cbp23us.zip](https://www2.census.gov/programs-surveys/cbp/datasets/2023/cbp23us.zip) — US Census Bureau, released 2025 (CBP 2023 still codes furniture stores as 2017-NAICS 442110; 449110 is the 2022-NAICS equivalent)
- **Confidence:** high (parsed from the Census flat file)
- **Use:** video-opener | submission-research

### F-industry-02 — California: 2,203 furniture stores, 94% with under 20 employees
- **Value:** 2,203 establishments, 18,322 employees, $1.00B payroll (NAICS 442110, March 2023). Size classes: <5 1,398; 5–9 441; 10–19 229; 20–49 92; 50–99 25; 100–249 9; 250–499 7. Under 10: 1,839 (83.5%); under 20: 2,068 (93.9%). BLS CES employment for the broader NAICS 4491 (furniture and home furnishings retailers) in California averaged 44,400 in 2024 and 42,900 in 2025.
- **Source:** [County Business Patterns 2023, state file cbp23st.zip](https://www2.census.gov/programs-surveys/cbp/datasets/2023/cbp23st.zip) — US Census Bureau, 2025; [FRED SMU06000004244910001](https://fred.stlouisfed.org/series/SMU06000004244910001) — BLS via FRED, 2026
- **Confidence:** high
- **Use:** submission-research | pitch

### F-industry-03 — 12,708 US furniture-store firms; 90% have under 20 employees and average $1.41M revenue; firms under 500 employees hold 45% of receipts
- **Value:** 2022: 12,708 firms, 22,286 establishments, $76.38B receipts. Firms with <20 employees: 11,441 firms (90.0%), 11,954 establishments (1.05 per firm, i.e., effectively single-location), $16.15B receipts ($1.41M per firm, 4.9 employees per firm). Firms <500 employees: 12,637 (99.4% of firms), $34.47B (45.1% of receipts). The 71 firms with 500+ employees run 6,598 establishments (29.6%) and take 54.9% of receipts.
- **Source:** [Statistics of U.S. Businesses 2022, us_state_6digitnaics_2022.txt](https://www2.census.gov/programs-surveys/susb/tables/2022/us_state_6digitnaics_2022.txt) — US Census Bureau, 2024
- **Confidence:** high (parsed from the Census file; "single-location" is inferred from 1.05 establishments per firm, not a direct single-unit count)
- **Use:** video-opener | submission-research | pitch

### F-industry-04 — California furniture-store firms: 1,390 firms, 90% under 20 employees, averaging $1.33M revenue
- **Value:** 2022: 1,390 firms, 2,223 establishments, $7.41B receipts. Firms <20 employees: 1,252 (90.1%), 1,319 establishments, $1.67B receipts ($1.33M per firm).
- **Source:** [Statistics of U.S. Businesses 2022 (state rows, FIPS 06)](https://www2.census.gov/programs-surveys/susb/tables/2022/us_state_6digitnaics_2022.txt) — US Census Bureau, 2024
- **Confidence:** high
- **Use:** submission-research | pitch

### F-industry-05 — US furniture-store sales $68.9B in 2024; furniture + home furnishings stores $125.0B
- **Value:** Sum of not-seasonally-adjusted monthly sales: NAICS 4421 furniture stores $75.8B (2022), $71.4B (2023), $68.9B (2024), $69.2B (2025); NAICS 442 furniture and home furnishings stores $136.8B (2022), $129.8B (2023), $125.0B (2024), $127.3B (2025). Census ARTS annual benchmark for 2022: 442 $143.6B, 4421 $79.9B. Trade press quoting the Commerce advance release put 2024 at $135.7B (different vintage/definition; medium).
- **Source:** [FRED MRTSSM4421USN](https://fred.stlouisfed.org/series/MRTSSM4421USN) and [FRED MRTSSM442USN](https://fred.stlouisfed.org/series/MRTSSM442USN) — Census Monthly Retail Trade via FRED, 2026; [ARTS 2022 sales.xlsx](https://www2.census.gov/programs-surveys/arts/tables/2022/sales.xlsx) — US Census Bureau; [Home Textiles Today, Jan 2025](https://www.hometextilestoday.com/industry-news/home-furnishes-stoes-finish-24-with-a-flourish-says-commerce-dept)
- **Confidence:** high for the Census/FRED series; medium for the trade-press $135.7B
- **Use:** video-opener | submission-research

### F-industry-06 — IBISWorld counts ~55,000 furniture-store businesses and a ~$167–170B market (broader definition)
- **Value:** 55,045 businesses and $169.8B market size in 2025 (search snapshot); page now shows 55,457 businesses (2026, +2.5%) and $166.8B (2026). California page: 9,020 establishments, 50,189 workers (2026). These counts include nonemployer and online sellers and exceed Census employer counts by ~2.5x.
- **Source:** [IBISWorld Furniture Stores in the US, number of businesses](https://www.ibisworld.com/united-states/number-of-businesses/furniture-stores/1016/), [market size](https://www.ibisworld.com/united-states/market-size/furniture-stores/1016/), [California](https://www.ibisworld.com/us/industry/california/furniture-stores/11095/) — IBISWorld, 2025–2026
- **Confidence:** medium (paywalled summary, definition differs from Census)
- **Use:** submission-research

### F-industry-07 — Gross margin of furniture and home furnishings stores: 51.0% of sales (2022)
- **Value:** 51.0% (2022), 51.0% (2021), 47.4% (2020), 48.6% (2019), 48.7% (2018); all-retail excluding autos 33.4% (2022).
- **Source:** [ARTS 2022, Estimated Annual Gross Margin as a Percentage of Sales by Kind of Business, gmper.xlsx](https://www2.census.gov/programs-surveys/arts/tables/2022/gmper.xlsx) — US Census Bureau, 2024
- **Confidence:** high (NAICS 442 level; no 4421 split published)
- **Use:** video-opener | layer1-spec | submission-research

### F-industry-08 — Independent-store survey medians: gross margin 50% (2019), 46.5% (2016), 43% (2004); stock turns 3 (2019), 4.0 (2016)
- **Value:** 2019: gross margin 50% (47% in 2018), median stock turns 3 (4 in 2018), advertising 10% of sales, delivery/design/other services 16% of revenue. 2016: gross margin 46.5%, turns 4.0, close ratio 22%, $200 sales per selling sq ft, 30,000 sq ft median selling space, 10 buyers per salesperson per week, 64 open hours/week. 2004 (300+ companies, two-thirds single-unit, 43% under $2M sales): gross margin 43% (bedroom 45%, upholstery 43–44%, bedding 44%), close ratio 36%, payroll 17% of revenue plus 3% benefits, sales per salesperson $434,782, net return on sales 3%.
- **Source:** [2019 Furniture Store Performance Report](https://www.furnituretoday.com/research-and-analysis/2019-furniture-store-performance-report) — Furniture Today, Nov 2019; [Close ratios and stock turns decrease; gross margin increases](https://www.furnituretoday.com/business-news/close-ratios-and-stock-turns-decrease-gross-margin-increases) — Furniture Today, Nov 2016; [Furniture store performance report](https://www.furnituretoday.com/business-news/furniture-store-performance-report) — Furniture Today, Jan 2005
- **Confidence:** medium (trade surveys of responding stores, sample sizes not stated for 2016/2019; 2004 data is old but is the only one with payroll and net-profit ratios)
- **Use:** submission-research | layer1-spec | pitch

### F-industry-09 — Public furniture retailers: gross margin 60.7% (Havertys 2024), 60.5% (Ethan Allen FY2025), 43.9% consolidated (La-Z-Boy FY2025, mostly wholesale)
- **Value:** Havertys 2024: net sales $722.9M, gross margin 60.7% (same as 2023), SG&A 58.0%, selling expenses $107.6M (14.9% of sales, "primarily compensation of sales team members", decline attributed to "lower commissioned-based compensation"), 129 stores averaging 35,000 sq ft, "commissioned-based sales team", in-house delivery. Ethan Allen FY2025: consolidated gross margin 60.5%, retail operating margin 3.8%, SG&A 50.4%, 142 company design centers, retail selling expenses down 4.8% "due to reduced delivery costs" and "lower designer variable compensation". La-Z-Boy FY2025: gross profit $926.4M on cost of sales $1,182.8M (43.9%), Retail segment sales $898.4M at 11.7% operating margin, 203 of 366 galleries company-owned.
- **Source:** [Havertys 10-K FY2024](https://www.sec.gov/Archives/edgar/data/216085/000162828025010869/hvt-20241231.htm) — SEC EDGAR, Mar 2025; [Ethan Allen 10-K FY2025](https://www.sec.gov/Archives/edgar/data/896156/000143774925027594/eth20250630_10k.htm) — SEC EDGAR, Aug 2025; [La-Z-Boy 10-K FY2025](https://www.sec.gov/Archives/edgar/data/57131/000005713125000029/lzb-20250426.htm) — SEC EDGAR, Jun 2025
- **Confidence:** high (10-K text); note public chains run higher gross margin than the 50% independent median because they own more of the chain
- **Use:** submission-research | pitch

### F-industry-10 — Inventory turns about 3 per year (~120 days of stock); Census-implied 3.1, Havertys 3.2, Ethan Allen 1.7
- **Value:** Census ARTS 2022: furniture and home furnishings stores held $22.5B of end-of-year inventory against $143.6B sales (15.7% of annual sales at retail, ~57 days of sales); at a 51% gross margin, cost of goods ≈ $70.4B, so implied turns ≈ 3.1x (≈117 days at cost). Havertys 2024: COGS $283.8M on average inventory $88.7M = 3.2x. Ethan Allen FY2025: COGS $242.5M on average inventory $141.5M = 1.7x (includes manufacturing inventory). Furniture Today median 3 (2019), 4.0 (2016).
- **Source:** [ARTS 2022 invent.xlsx](https://www2.census.gov/programs-surveys/arts/tables/2022/invent.xlsx) and [sales.xlsx](https://www2.census.gov/programs-surveys/arts/tables/2022/sales.xlsx) — US Census Bureau; Havertys and Ethan Allen 10-Ks as in F-industry-09; Furniture Today reports as in F-industry-08
- **Confidence:** high for inputs; the turn ratios are computed (year-end inventory, not average) and labeled as such
- **Use:** layer1-spec | submission-research | demo-data

### F-industry-11 — Markdowns cost US non-grocery retailers ~$300B (12% of sales); 53% of unplanned markdowns trace to inventory misjudgment; only 60% of inventory sells at full price
- **Value:** 2018: ~$300B lost revenue, ~12% of non-grocery retail sales, model assumes 30% average discount; 53% of unplanned markdown cost from inventory misjudgment; average full-price sell-through 60%; only 15% of respondents sold 90–100% at full price. Survey of 200 senior US retail decision makers, Oct 2018.
- **Source:** [US Retailer Survey: Revealing the Hidden Costs of Poor Inventory Management](https://coresight.com/research/us-retailer-survey-revealing-the-hidden-costs-of-poor-inventory-management-2/) — Coresight Research with Celect, Feb 2019
- **Confidence:** medium (survey extrapolation, all non-grocery retail, not furniture-specific)
- **Use:** submission-research | pitch

### F-industry-12 — Inventory carrying cost: 20–30% of inventory value per year (standard range; weakly sourced)
- **Value:** 20–30% per year, attributed to APQC benchmarking and ISM; worked example at 25% = capital 10% + storage 7% + insurance/taxes 2% + obsolescence/shrink/damage 6%. Wikipedia states the same 20–30% range with a "citation needed" tag.
- **Source:** [Carrying Costs glossary](https://sixsigmadsi.com/glossary/carrying-costs/) — Six Sigma Development Solutions, 2024; [Carrying cost](https://en.wikipedia.org/wiki/Carrying_cost) — Wikipedia, 2026
- **Confidence:** low-medium (the range is universal in practice but no primary study was reachable; treat as a convention, not a measurement)
- **Use:** layer1-spec | submission-research

### F-industry-13 — Pay models: nearly half of full-time furniture salespeople are commission-only (2016); by 2019 hourly+commission 29%, salary+commission 28%, salary-only 28%
- **Value:** 2016: ~50% commission-only, 21% hourly plus commission, 17% salary plus commission. 2019: hourly-plus-commission 29%, salary-plus-commission 28%, salary-only 28% of responding stores.
- **Source:** Furniture Today 2016 and 2019 performance reports (links in F-industry-08)
- **Confidence:** medium (trade survey)
- **Use:** submission-research | pitch

### F-industry-14 — Commission rates: typically 4–8% of the sale, up to 10%; quoted independent plan pays 6% (3% on closeouts); draw-against-commission is the common mechanism
- **Value:** Career guide: 4–8% at most stores, up to 10% at high-end stores, average pay ~$30,000. Home Furnishings Business (2014): DoMa Home Furnishings pays 6% once a $30,000 monthly minimum is met and 3% on closeouts ("I gave up margin, so they give up margin"); Sklar Furnishings uses a weekly draw with monthly commission; trainer Jeff Hiller says big stores expect ~$800,000 per salesperson per year earning $40–50k (≈5–6% effective), top performers $80–100k, and suggests $26–30k base plus bonus for mid-size stores. Current postings: 12-week salary guarantee then weekly draw plus escalating commission (Royal Furniture), $14/hr plus commission draw (Express Employment, Pensacola), "base salary is essentially an advance against future commissions" (Paylocity sales-consultant postings).
- **Source:** [Furniture Salesman salary](https://www.shmoop.com/careers/furniture-salesman/salary.html) — Shmoop, n.d.; [Balancing Act](https://hfbusiness.com/CurrentIssue/CurrentIssueModule/ArticleId/10207/balancing-act) — Home Furnishings Business, Jan 2014; [Sales Consultant posting](https://recruiting.paylocity.com/Recruiting/Jobs/Details/3921631) — Paylocity, 2025; [Sales Associate posting](https://jobs.expresspros.com/job/14543887) — Express Employment, 2025
- **Confidence:** medium (no published rate survey; triangulated from a trade article, a career guide and job ads)
- **Use:** layer1-spec | submission-research | demo-data

### F-industry-15 — Havertys: selling expense (mostly sales compensation) 14.9% of sales; independents' total payroll 17% of revenue (2004 median)
- **Value:** Havertys 2024 selling expenses $107.6M on $722.9M sales; Furniture Today 2004 median payroll 17% + benefits 3%.
- **Source:** Havertys 10-K (F-industry-09); Furniture Today 2005 (F-industry-08)
- **Confidence:** high / medium
- **Use:** demo-data | layer1-spec

### F-industry-16 — Revenue-based commission rewards discounting: at 50% margin and 6% commission, a 10% discount costs the rep 10% of pay but the store 20% of gross profit
- **Value:** Arithmetic on sourced ratios: $2,000 ticket at 50% gross margin (F-industry-07) and 6% commission (F-industry-14): full price → rep $120, store gross profit $1,000; 10% off → rep $108 (−10%), store $800 (−20%); 20% off → rep $96 (−20%), store $600 (−40%). Practitioner sources state the same conflict: at a 40% margin a 10%-of-revenue commission is 25% of margin "and it pays reps to discount"; margin-based plans are common in distribution and channel sales.
- **Source:** [Paying sales commissions on revenues vs. profit](https://www.peaksalesrecruiting.com/blog/paying-sales-commissions-on-revenues-vs-profit/) — Peak Sales Recruiting, n.d.; [Commission structure based on gross profit](https://qobra.co/blog/commission-structure-based-on-gross-profit) — Qobra, n.d.
- **Confidence:** high for the arithmetic; low-medium for the practitioner claims (no controlled study found)
- **Use:** pitch | layer1-spec

### F-industry-17 — 71% of consumers who haggled over furniture got a discount (2009); furniture, antiques and appliances were the top-success categories (2013)
- **Value:** 2009 (n=1,002 adults): 66%+ tried to negotiate in the past six months; success among hagglers: furniture 71%, appliances 75%, electronics 71%, hotels 83%. 2013 (n=2,000): 48% tried bargaining in the past three years (61% in 2007); 89% of hagglers got a discount at least once; highest success with collectibles/antiques, furniture, appliances.
- **Source:** [Haggling for everything is new rule in a down economy](https://www.consumerreports.org/media-room/press-releases/2009/05/consumer-reports-money-special-publication-haggling-for-everything-is-new-rule-in-a-down-economy) — Consumer Reports, May 2009; [Consumer Reports haggling survey press release](https://www.consumerreports.org/media-room/press-releases/2013/07/my-entry) — Consumer Reports, Jul 2013
- **Confidence:** high for the numbers, but 13–17 years old
- **Use:** video-opener | submission-research

### F-industry-18 — Average saving from haggling over furniture: ~$300 per purchase (2013)
- **Value:** "Those who haggled over furniture and questioned a health-related charge saved an average of $300"; appliances $200; antiques $100; phone plan $80.
- **Source:** Consumer Reports 2013 press release (link in F-industry-17); corroborated by [ABC13 coverage](https://abc13.com/archive/9161775) — KTRK, 2013
- **Confidence:** medium (figure is shared across two categories in the release)
- **Use:** video-opener | layer1-spec

### F-industry-19 — 60% of 2025 furniture buyers say they paid more than they consider acceptable
- **Value:** L.E.K. Consulting national survey of 2,000 US adults, summer 2025: 60% of past-12-month furniture buyers paid above their acceptable level (dining tables 66%, sofas 62%, mattresses 61%); 83% would trade down on durable goods.
- **Source:** [Side effect of tariff fatigue: furniture shoppers are trading down, survey finds](https://www.designerstoday.com/furniture/side-effect-of-tariff-fatigue-furniture-shoppers-are-trading-down-survey-finds) — Designers Today, Oct 2025
- **Confidence:** medium (trade-press summary of a consultancy survey)
- **Use:** pitch | submission-research

### F-industry-20 — Delivery cost drives defection: 56% would avoid a boutique retailer over shipping cost; ~40% would switch to Amazon/Wayfair without free shipping; 27% have abandoned a cart over delivery expense
- **Value:** uShip/YouGov 2019, 330 buyers of an oversized furniture item in the prior year. Separately, PYMNTS/Elastic Path 2022 (n=2,094): 47% abandoned a home-furnishing purchase in the past 12 months; of those, 37% cited delivery cost too high, 40% found it cheaper elsewhere.
- **Source:** [Impatient customers, paying nothing for something](https://about.uship.com/uncategorized/impatient-customers-paying-nothing-for-something-heavy-goods-shippers-face-same-e-commerce-delivery-pressures-as-smaller-stuff/) — uShip, Sep 2019; [54% of clothing shoppers have abandoned a cart](https://pymnts.com/?p=1353688) — PYMNTS, Jul 2022
- **Confidence:** medium (vendor-commissioned survey; small sample)
- **Use:** pitch | submission-research

### F-industry-21 — Consumers will pay only 1–5% extra for faster furniture delivery and resist surcharges above 10%
- **Value:** Furniture Today Strategic Insights, Jan 2021, n=515: typical acceptable surcharge 1–5% of price; most resist above 10%; mattresses (27.4%) and sofas (27%) are the items buyers would most pay to get faster.
- **Source:** [Delivery fees for faster service resonate best with bigger items](https://www.furnituretoday.com/research-and-analysis/delivery-fees-for-faster-service-resonate-best-with-bigger-items) — Furniture Today, May 2021
- **Confidence:** medium
- **Use:** layer1-spec

### F-industry-22 — Havertys 2024: delivery cost $37.1M (5.1% of sales) vs delivery-fee revenue $29.3M (4.0%); fees recovered 79%, net subsidy 1.1% of sales; warehouse/delivery/transport $60.8M (8.4%)
- **Value:** From Note 2 of the 10-K: delivery costs in SG&A $37,085K (2024) / $42,361K (2023); delivery fee revenue included in net sales $29,279K / $36,187K; warehouse, delivery and transportation $60,810K / $74,442K; net sales $722.9M. Havertys does "not outsource the delivery function".
- **Source:** [Havertys 10-K FY2024](https://www.sec.gov/Archives/edgar/data/216085/000162828025010869/hvt-20241231.htm) — SEC EDGAR, Mar 2025
- **Confidence:** high
- **Use:** video-opener | layer1-spec | submission-research

### F-industry-23 — Trade view: delivery income adds 1–2% to the bottom line; charging for delivery has been the norm for ~25 years; 20–30% of customers pick up
- **Value:** Home Furnishings Business column, Mar 2016: delivery income 1–2% of bottom line; finding 1–2 points of margin to absorb free delivery is "daunting"; 20–30% customer pickup.
- **Source:** [Delivery on the House](https://hfbusiness.com/CurrentIssue/CurrentIssueModule/ArticleID/13923/delivery-on-the-house) — Home Furnishings Business, Mar 2016
- **Confidence:** medium (opinion column, no data table)
- **Use:** layer1-spec | pitch

### F-industry-24 — Delivery price points and crew cost inputs: retail white-glove from $59 (Ethan Allen) to $199 (RH); last-mile provider revenue <$90 per shipment, $50 for a bedroom set up to $250 with setup; delivery helpers earn ~$17.60–18/hr; two-person crew with truck $100–200/hr on moving marketplaces
- **Value:** Consumer Reports cites Ethan Allen white-glove from $59 on orders up to $499 and RH flat rates from $199 within 50 miles. Armstrong & Associates (via Inbound Logistics): last-mile revenue averages under $90/shipment; a bedroom set ~$50, ~$250 with installation; big-and-bulky crews run 6–12 stops a day (Racklify). Job postings: delivery helper $17.60/hr (Tacoma, WA) and $18/hr (Indiana). Airtasker: two-person furniture-moving crew with truck typically $100–200/hr.
- **Source:** [Make furniture delivery and returns as hassle-free as possible](https://www.consumerreports.org/furniture/make-furniture-delivery-and-returns-as-hassle-free-as-possible-a5212662749/) — Consumer Reports (paywalled; figures from search excerpt); [Last-Mile Deliveries Grow Bigger and Bulkier](https://www.inboundlogistics.com/articles/last-mile-deliveries-grow-bigger-and-bulkier/) — Inbound Logistics (figures from search excerpt; direct fetch blocked); [Home goods delivery costs](https://racklify.com/encyclopedia/home-goods-delivery-costs-and-operational-tips-for-3pls/) — Racklify; [Delivery Helper, Tacoma](https://www.militaryhire.com/jobs-for-veterans/job/8413205/Delivery-Helper/state/Washington/city/Tacoma/); [Delivery Helper, Express Employment](https://jobs.expresspros.com/job/14536538); [Furniture moving cost](https://www.airtasker.com/us/costs/furniture-movers/furniture-moving-cost/) — Airtasker
- **Confidence:** low-medium (mixed retailer prices, 3PL revenue and marketplace rates; no published per-stop in-house cost)
- **Use:** demo-data | layer1-spec

### F-industry-25 — Price-change labor is measurable: $0.52 per price change, 0.70% of revenue, 35% of net margin (supermarkets, 1991–92); vendor rule of thumb 1–2 minutes per paper tag change at $20–25/hr loaded
- **Value:** Levy, Bergen, Dutta and Venable: menu costs average $105,887 per store per year, 0.70% of revenues, 35.2% of net margins, $0.52 per price change ($1.33 where item-pricing laws require a tag on every item); chains skipped 20–30% of cost-justified price changes because of the cost. ShopAppy (retail trade site, vendor-sourced): 1–2 minutes per change including print, walk and hang; $20–25/hr loaded; 100 labor hours/week at 4,000 changes.
- **Source:** [The Magnitude of Menu Costs: Direct Evidence from Large U.S. Supermarket Chains](https://econwpa.ub.uni-muenchen.de/econ-wp/mac/papers/0505/0505012.pdf) — Levy et al., Quarterly Journal of Economics 1997 (working-paper copy); [Electronic shelf labels in grocery: cost, payback and pricing rules](https://shopappy.com/retail/supermarkets-grocers/electronic-shelf-labels-grocery) — ShopAppy, 2025 (vendor-sourced estimates)
- **Confidence:** high for the academic study (but grocery, 1990s dollars); low for the vendor rule of thumb
- **Use:** submission-research | layer1-spec

### F-industry-26 — Retail rent context: Los Angeles $2.86/sq ft/month NNN (~$34/yr) in Q4 2025; Bay Area $33.18/sq ft/yr NNN in Q1 2025
- **Value:** CBRE Los Angeles Q4 2025: average asking rent $2.86 NNN monthly, availability 6.2%; Westside $4.31, San Gabriel Valley $2.12. CBRE Bay Area Q1 2025: $33.18/sq ft/yr NNN, vacancy 5.7%. A 30,000 sq ft showroom (Furniture Today 2016 median) at $34/sq ft/yr = ~$1.0M/yr before NNN charges; at $2.12 (San Gabriel Valley) = $763k.
- **Source:** [Q4 2025 LA Retail Figures](https://mktgdocs.cbre.com/2299/2047f204-1f0b-44cd-9d36-81b5a093cccb-2058784801/Q4_2025_LA_Retail_Figures.pdf) — CBRE Research, Jan 2026; [Bay Area Retail Figures Q1 2025](https://www.cbre.com/insights/figures/bay-area-retail-figures-q1-2025) — CBRE, Apr 2025 (figure from search excerpt; page did not render on fetch)
- **Confidence:** high (LA, read from the PDF); medium (Bay Area)
- **Use:** submission-research | demo-data

### F-industry-27 — Microbusiness owners: 62% work more than 50 hours a week, median 60 hours (2024); 20% took no vacation in a year (2014)
- **Value:** UENI, May 2024, 837 US businesses with five or fewer employees: 62% over 50 hours/week (same share as a 2005 Wells Fargo/Gallup poll), median 60 hours; 22.4% of time on admin/legal/compliance; only 29% have a time-management strategy. Sam's Club/Gallup Microbusiness Tracker, May 2014, n=1,004: 20% took no vacation days in 12 months, another 21% a week or less; average 39 hours/week (42 among no-vacation owners).
- **Source:** [How microbusiness owners spend their time](https://ueni.com/en-us/small-business-research/how-microbusiness-owners-spend-their-time) — UENI, 2024; [One in Five Microbusiness Owners Took No Vacation Last Year](https://news.gallup.com/poll/172889/one-five-microbusiness-owners-took-no-vacation-last-year.aspx) — Gallup, Jul 2014
- **Confidence:** medium (general SMB, not furniture; UENI is a vendor survey, Gallup is reputable but old)
- **Use:** video-opener | pitch

### F-industry-28 — Furniture Today Top 100 sold $51.6B in 2024, down 8%; three bankruptcies removed 2,300+ stores
- **Value:** Top 100 furniture, bedding and accessories sales $51.6B (2024) vs $56.1B (2023) and $60.6B (2022); Big Lots, American Freight and Conn's/Badcock exited; Top 100 store count fell 20.9% (2,400+ units). Context for independents: Census SUSB shows firms under 500 employees hold 45% of furniture-store receipts (F-industry-03).
- **Source:** [Still struggling: In 2024, Top 100 continued its sales decline](https://www.furnituretoday.com/furniture-retailing/still-struggling-in-2024-top-100-continued-its-sales-decline) — Furniture Today, May 2025
- **Confidence:** medium (trade ranking; not directly comparable to Census store sales)
- **Use:** pitch

## Tables

### Headline numbers for the 2-minute video

| # | Number | What it says | Source (year) |
|---|---|---|---|
| 1 | 21,964 US furniture stores; 91.5% have under 20 employees | This is a small-shop industry | Census CBP 2023 [F-industry-01] |
| 2 | 90% of 12,708 furniture-store firms are under 20 employees, averaging $1.4M revenue; firms under 500 employees hold 45% of sales | Independents are the market, not a niche | Census SUSB 2022 [F-industry-03] |
| 3 | $68.9B furniture-store sales; $125B with home furnishings (2024) | The dollars at stake | Census MRTS via FRED [F-industry-05] |
| 4 | 51% gross margin | Each 1 point of discount is ~2% of gross profit | Census ARTS 2022 [F-industry-07] |
| 5 | ~3 inventory turns a year (~120 days of stock) | Stock sits; aged pieces are the norm | Furniture Today 2019; ARTS-derived [F-industry-10] |
| 6 | 71% of furniture hagglers win; average saving ~$300 | Customers negotiate and expect to win | Consumer Reports 2009, 2013 [F-industry-17, 18] |
| 7 | Even Havertys recovers only 79% of delivery cost through fees; delivery is 5.1% of sales | "Free delivery" is a real margin leak | Havertys 10-K 2024 [F-industry-22] |
| 8 | 62% of microbusiness owners work 50+ hours; median 60 | The owner cannot be on the floor for every deal | UENI 2024 [F-industry-27] |
| CA | 2,203 California furniture stores (94% under 20 employees); 1,390 firms averaging $1.33M | Local framing for VibeCon SF | Census CBP 2023, SUSB 2022 [F-industry-02, 04] |

### Worked example: annual margin leakage, one store ($500k inventory at cost, 3 sales staff, 2 delivery staff)

Every row uses a sourced ratio or an explicitly labeled assumption (A). Dollar results are estimates, not measurements.

| Line | Input | Value | Basis |
|---|---|---|---|
| Store size | Inventory at cost | $500,000 | Given |
| | Inventory turns | 3.0 / yr | Furniture Today 2019 median 3; ARTS-derived 3.1 [F-industry-10] |
| | Cost of goods sold | $1,500,000 | $500k × 3.0 |
| | Gross margin | 50% | ARTS 2022 51%; FT 2019 50% [F-industry-07, 08] |
| | Annual sales / gross profit | $3,000,000 / $1,500,000 | COGS ÷ (1 − 0.50). Implies $1.0M per salesperson, above the $435k (2004 median) to $800k (big-store target) norms, so this store is at the high end; see sensitivity |
| | Average ticket | $2,000 (A) | Assumption; no published independent-store average ticket found |
| | Tickets per year | 1,500 | Sales ÷ ticket |
| L1 Negotiated discounts | Share of tickets with a concession | 40% (A) | Bracketed by CR 2009 (66% of adults haggled on something in 6 months; 71% of furniture hagglers won) and CR 2013 (48% haggled in 3 years) [F-industry-17] |
| | Average concession | $300 | CR 2013 average furniture saving [F-industry-18] |
| | Gross exposure | $180,000 (6.0% of sales, 12% of gross profit) | 600 × $300 |
| | Avoidable share | 1/3 (A) → $60,000 | Assumption: the part given beyond the owner's intended floor; a guardrail tool targets this slice |
| L2 Waived delivery fees | Deliveries per year | 1,125 | 75% of tickets delivered (HFB: 20–30% pick up) [F-industry-23] |
| | Standard delivery fee | $99 (A) | Between Ethan Allen from $59 and RH $199 [F-industry-24] |
| | Fee waived by staff | 40% (A) → 450 | Assumption anchored on ~40% of buyers saying they defect without free shipping [F-industry-20] |
| | Leak | $44,550 (1.5% of sales) | 450 × $99. Cross-check: Havertys' net delivery subsidy is 1.1% of sales [F-industry-22] |
| | Cash cost per stop (context) | ~$105 | 2 staff × 2,080 h × $18/h [F-industry-24] × 1.25 burden (A) = $93,600, plus truck $24,000/yr (A) = $117,600 ÷ 1,125 stops |
| L3 Aged-stock carrying cost | Aged share of inventory | 20% (A) = $100,000 at cost | Assumption; no furniture benchmark found (Gaps) |
| | Carrying cost rate | 25% / yr | Midpoint of 20–30% [F-industry-12] |
| | Leak | $25,000 | $100k × 25% |
| L4 Clearance markdowns on aged stock | Retail value of aged stock | $200,000 | $100k cost at 50% margin |
| | Clearance discount | 30% | Coresight assumed average markdown [F-industry-11] |
| | Gross margin given up | $60,000 | $200k × 30% |
| | Avoidable share | 53% → $31,800 | Coresight: 53% of unplanned markdown cost comes from inventory misjudgment [F-industry-11] |
| L5 Re-tagging labor | Price changes | 1,500 tags × 4 changes/yr (A) = 6,000 | Assumption on frequency |
| | Time and wage | 1.5 min × $20/h | ShopAppy vendor rule of thumb [F-industry-25] |
| | Leak | $3,000 | 150 h × $20 |
| L6 Commission asymmetry (mechanism, not a separate dollar line) | 6% of revenue vs 50% margin | A 10% discount costs the rep 10% of commission and the store 20% of gross profit | [F-industry-16] |
| **Total gross exposure** | L1 + L2 + L3 + L4 + L5 | **$312,550 ≈ 10.4% of sales ≈ 21% of gross profit** | |
| **Avoidable estimate** | L1 avoidable + L2 + L3 + L4 avoidable + L5 | **$164,350 ≈ 5.5% of sales ≈ 11% of gross profit** | |
| Reference: typical net profit | 3% net return on sales | $90,000 | Furniture Today 2004 median [F-industry-08]; the avoidable leak is ~1.8× this |
| Sensitivity | At 2.0 turns ($2.0M sales, 1,000 tickets) | Exposure ≈ $225k; avoidable ≈ $125k | L1, L2, L5 scale with tickets; L3, L4 are inventory-based and unchanged |

One-line version: a $3M independent furniture store with $500k of stock plausibly exposes ~$310k a year (about a fifth of gross profit) to negotiated discounts, waived delivery and aged stock, of which roughly $165k (5.5% of sales, almost twice a typical 3% net profit) is the avoidable slice a guardrail tool targets; every ratio is sourced, the share assumptions are labeled.

## Gaps and unverified
- Web-search budget for the session was exhausted part-way; the following were not found and should be re-tried: HFA or Furniture Today operating survey with delivery charge norms and commission rates; Furniture Today 2020–2025 performance reports (newest found is 2019); Economic Census 2022 single-unit vs multi-unit counts for 449110 (SUSB establishments-per-firm is used as the proxy).
- Aged inventory: no furniture-specific benchmark for share of stock over 90/180 days or write-down rates; the 20% aged share in the worked example is an assumption. Public 10-Ks do not disclose it.
- Commission rates: no published survey; 4–8% (career guide), 6% (one retailer quoted in 2014) and job ads are the evidence. Commission-on-margin vs commission-on-revenue: no controlled study found, only practitioner sources and arithmetic.
- Haggling: newest Consumer Reports data is 2013; the furniture $300 saving is shared with "health-related charge" in the release. No survey of how often furniture salespeople use free delivery as a closer was found; the uShip 40% figure is buyer intent, not retailer behavior.
- Delivery cost per stop for an in-house two-person crew: no published figure; the ~$105 is built from wage postings plus assumed burden and truck cost. BLS OEWS wage pages (NAICS 449100) returned 403 and could not be read.
- Initial markup vs maintained margin: only forum anecdotes (2.0–2.5× cost) and definitions (Toolio) were found; not included as a finding. ARTS 51% gross margin implies a maintained markup of ~2.04× cost.
- Average revenue per independent store: SUSB firm receipts (<20 employees: $1.41M US, $1.33M CA) is the best available; it is per firm, not per store, and 2022.
- Owner time on the floor / inability to delegate in furniture retail: nothing furniture-specific; UENI 2024 and Gallup 2014 are general microbusiness data.
- Carrying-cost 20–30%: convention without a reachable primary study (Investopedia and NetSuite pages were blocked).
- IBISWorld and CBRE Bay Area figures come from paywalled or non-rendering pages via search excerpts; marked medium.
- 2024 NAICS 442 sales: Census/FRED sum $125.0B vs trade-press $135.7B (advance release, different vintage/definition); the FRED series is used.

## Sources
1. County Business Patterns 2023, US file — US Census Bureau, 2025 — https://www2.census.gov/programs-surveys/cbp/datasets/2023/cbp23us.zip
2. County Business Patterns 2023, state file — US Census Bureau, 2025 — https://www2.census.gov/programs-surveys/cbp/datasets/2023/cbp23st.zip
3. Statistics of U.S. Businesses 2022, US and state by 6-digit NAICS — US Census Bureau, 2024 — https://www2.census.gov/programs-surveys/susb/tables/2022/us_state_6digitnaics_2022.txt
4. Annual Retail Trade Survey 2022, gross margin as a percentage of sales — US Census Bureau — https://www2.census.gov/programs-surveys/arts/tables/2022/gmper.xlsx
5. Annual Retail Trade Survey 2022, end-of-year inventories — US Census Bureau — https://www2.census.gov/programs-surveys/arts/tables/2022/invent.xlsx
6. Annual Retail Trade Survey 2022, annual sales — US Census Bureau — https://www2.census.gov/programs-surveys/arts/tables/2022/sales.xlsx
7. Retail Sales: Furniture Stores (MRTSSM4421USN) — Census via FRED, 2026 — https://fred.stlouisfed.org/series/MRTSSM4421USN
8. Retail Sales: Furniture and Home Furnishings Stores (MRTSSM442USN) — Census via FRED, 2026 — https://fred.stlouisfed.org/series/MRTSSM442USN
9. All Employees: Furniture and Home Furnishings Retailers in California (SMU06000004244910001) — BLS via FRED, 2026 — https://fred.stlouisfed.org/series/SMU06000004244910001
10. Haverty Furniture Companies 10-K FY2024 — SEC EDGAR, Mar 2025 — https://www.sec.gov/Archives/edgar/data/216085/000162828025010869/hvt-20241231.htm
11. Havertys Q4 2024 results, Exhibit 99 — SEC EDGAR, Feb 2025 — https://www.sec.gov/Archives/edgar/data/216085/000021608525000002/hvtex99.htm
12. La-Z-Boy 10-K FY2025 — SEC EDGAR, Jun 2025 — https://www.sec.gov/Archives/edgar/data/57131/000005713125000029/lzb-20250426.htm
13. Ethan Allen Interiors 10-K FY2025 — SEC EDGAR, Aug 2025 — https://www.sec.gov/Archives/edgar/data/896156/000143774925027594/eth20250630_10k.htm
14. 2019 Furniture Store Performance Report — Furniture Today, Nov 2019 — https://www.furnituretoday.com/research-and-analysis/2019-furniture-store-performance-report
15. Close ratios and stock turns decrease; gross margin increases — Furniture Today, Nov 2016 — https://www.furnituretoday.com/business-news/close-ratios-and-stock-turns-decrease-gross-margin-increases
16. Furniture store performance report (2004 data) — Furniture Today, Jan 2005 — https://www.furnituretoday.com/business-news/furniture-store-performance-report
17. Still struggling: In 2024, Top 100 continued its sales decline — Furniture Today, May 2025 — https://www.furnituretoday.com/furniture-retailing/still-struggling-in-2024-top-100-continued-its-sales-decline
18. Balancing Act (sales compensation) — Home Furnishings Business, Jan 2014 — https://hfbusiness.com/CurrentIssue/CurrentIssueModule/ArticleId/10207/balancing-act
19. Delivery on the House — Home Furnishings Business, Mar 2016 — https://hfbusiness.com/CurrentIssue/CurrentIssueModule/ArticleID/13923/delivery-on-the-house
20. Furniture Salesman salary — Shmoop, n.d. — https://www.shmoop.com/careers/furniture-salesman/salary.html
21. Sales Consultant posting (draw against commission) — Paylocity, 2025 — https://recruiting.paylocity.com/Recruiting/Jobs/Details/3921631
22. Sales Associate posting ($14/hr + commission draw) — Express Employment, 2025 — https://jobs.expresspros.com/job/14543887
23. Paying sales commissions on revenues vs. profit — Peak Sales Recruiting, n.d. — https://www.peaksalesrecruiting.com/blog/paying-sales-commissions-on-revenues-vs-profit/
24. Commission structure based on gross profit — Qobra, n.d. — https://qobra.co/blog/commission-structure-based-on-gross-profit
25. Haggling for everything is new rule in a down economy — Consumer Reports, May 2009 — https://www.consumerreports.org/media-room/press-releases/2009/05/consumer-reports-money-special-publication-haggling-for-everything-is-new-rule-in-a-down-economy
26. Consumer Reports haggling survey press release — Consumer Reports, Jul 2013 — https://www.consumerreports.org/media-room/press-releases/2013/07/my-entry
27. Haggling coverage of the 2013 survey — ABC13/KTRK, 2013 — https://abc13.com/archive/9161775
28. Side effect of tariff fatigue: furniture shoppers are trading down (L.E.K. survey) — Designers Today, Oct 2025 — https://www.designerstoday.com/furniture/side-effect-of-tariff-fatigue-furniture-shoppers-are-trading-down-survey-finds
29. Impatient customers, paying nothing for something (uShip/YouGov) — uShip, Sep 2019 — https://about.uship.com/uncategorized/impatient-customers-paying-nothing-for-something-heavy-goods-shippers-face-same-e-commerce-delivery-pressures-as-smaller-stuff/
30. 54% of clothing, accessory shoppers have abandoned an online cart (Elastic Path study) — PYMNTS, Jul 2022 — https://pymnts.com/?p=1353688
31. Delivery fees for faster service resonate best with bigger items — Furniture Today, May 2021 — https://www.furnituretoday.com/research-and-analysis/delivery-fees-for-faster-service-resonate-best-with-bigger-items
32. Make furniture delivery and returns as hassle-free as possible — Consumer Reports (paywalled) — https://www.consumerreports.org/furniture/make-furniture-delivery-and-returns-as-hassle-free-as-possible-a5212662749/
33. Last-Mile Deliveries Grow Bigger and Bulkier (Armstrong & Associates data) — Inbound Logistics — https://www.inboundlogistics.com/articles/last-mile-deliveries-grow-bigger-and-bulkier/
34. Home goods delivery costs and operational tips for 3PLs — Racklify — https://racklify.com/encyclopedia/home-goods-delivery-costs-and-operational-tips-for-3pls/
35. Delivery Helper posting, Tacoma WA ($17.60/hr) — MilitaryHire — https://www.militaryhire.com/jobs-for-veterans/job/8413205/Delivery-Helper/state/Washington/city/Tacoma/
36. Delivery Helper posting ($18/hr) — Express Employment — https://jobs.expresspros.com/job/14536538
37. Furniture moving cost (two-person crew rates) — Airtasker — https://www.airtasker.com/us/costs/furniture-movers/furniture-moving-cost/
38. The Magnitude of Menu Costs: Direct Evidence from Large U.S. Supermarket Chains — Levy, Bergen, Dutta, Venable, QJE 1997 (working paper copy) — https://econwpa.ub.uni-muenchen.de/econ-wp/mac/papers/0505/0505012.pdf
39. Electronic shelf labels in grocery: cost, payback and pricing rules — ShopAppy, 2025 — https://shopappy.com/retail/supermarkets-grocers/electronic-shelf-labels-grocery
40. Carrying Costs glossary — Six Sigma Development Solutions, 2024 — https://sixsigmadsi.com/glossary/carrying-costs/
41. Carrying cost — Wikipedia, 2026 — https://en.wikipedia.org/wiki/Carrying_cost
42. US Retailer Survey: Revealing the Hidden Costs of Poor Inventory Management — Coresight Research, Feb 2019 — https://coresight.com/research/us-retailer-survey-revealing-the-hidden-costs-of-poor-inventory-management-2/
43. Q4 2025 Los Angeles Retail Figures — CBRE Research, Jan 2026 — https://mktgdocs.cbre.com/2299/2047f204-1f0b-44cd-9d36-81b5a093cccb-2058784801/Q4_2025_LA_Retail_Figures.pdf
44. Bay Area Retail Figures Q1 2025 — CBRE, Apr 2025 — https://www.cbre.com/insights/figures/bay-area-retail-figures-q1-2025
45. Furniture Stores in the US, number of businesses — IBISWorld, 2026 — https://www.ibisworld.com/united-states/number-of-businesses/furniture-stores/1016/
46. Furniture Stores in the US, market size — IBISWorld, 2026 — https://www.ibisworld.com/united-states/market-size/furniture-stores/1016/
47. Furniture Stores in California — IBISWorld, 2026 — https://www.ibisworld.com/us/industry/california/furniture-stores/11095/
48. How microbusiness owners spend their time — UENI, May 2024 — https://ueni.com/en-us/small-business-research/how-microbusiness-owners-spend-their-time
49. One in Five Microbusiness Owners Took No Vacation Last Year — Gallup, Jul 2014 — https://news.gallup.com/poll/172889/one-five-microbusiness-owners-took-no-vacation-last-year.aspx
50. Home furnishings stores finish '24 with a flourish, says Commerce Dept — Home Textiles Today, Jan 2025 — https://www.hometextilestoday.com/industry-news/home-furnishes-stoes-finish-24-with-a-flourish-says-commerce-dept
