# Pricing layers — every input that moves tag price and floor
Generated: 2026-10-24 · Agent: research-pricing · Status: complete (vendor-specific MAP terms unsourced; see Gaps)

Scope: independent furniture gallery (new branded mid-to-upper goods, some special order, California, own delivery crew). "Tag" = initial ticketed price. "Floor" = lowest negotiated price the owner will accept. Owner statements from `01-furniture-pricing-system.md` (A-S, B-S, C-P IDs) are treated as hypotheses, not facts, and are flagged where they agree or disagree with sources.

## Summary

- Cost basis is landed cost (invoice + inbound freight + duties/tariffs + insurance), allocated per item by cost share, cube, or weight; the 25% Section 232 tariff on imported upholstered furniture (Oct 2025) is now part of that basis [F-pricing-01, F-pricing-02, F-pricing-03].
- Keystone (2.0x) is the industry anchor, but published independents' medians are below it on realized margin (46–47% gross margin ≈ 1.85–1.9x), while a well-run chain (Havertys) reports 60.7% ≈ 2.5x; the owner's 1.5x/1.8x/2x examples (C-P039) sit inside the sourced range [F-pricing-05, F-pricing-06, F-pricing-07, F-pricing-09].
- MAP restricts advertised price only; in-store selling below MAP is legal. Unilateral minimum retail price policies (Tempur-Pedic, Ekornes/Stressless) do bind the floor, because the vendor can cut off supply [F-pricing-11, F-pricing-12, F-pricing-13].
- Age is the one input with a sourced, mechanical effect: carrying cost 15–35%/yr plus rent of ~$33–37/sq ft/yr NNN in CA metros means a 3-year-old piece has consumed a measurable share of its margin; general-retail playbooks step markdowns at 90/180/270–365 days [F-pricing-04, F-pricing-26, F-pricing-38].
- Negotiation is normal in furniture: furniture hagglers saved ~$300 on average, 89% of hagglers overall succeeded, and 60% of 2025 furniture buyers felt they overpaid; independents are reported as more negotiable than chains [F-pricing-23, F-pricing-34].
- Legal guardrail is firm: California B&P §17501 requires a "former price" to have been the prevailing price within the prior three months (or dated), and FTC 16 CFR 233 requires a bona fide former price offered for a reasonably substantial period. The owner's "raise the tag to $300, cross it out, sell at $200" idea (B-S156–197) is exactly what these rules prohibit [F-pricing-39, F-pricing-42].

## Findings

### Layer 1 — Cost basis

### F-pricing-01 — Landed cost = material cost + freight + landed add-ons (insurance, customs, duties, tariffs)
- **Value:** Definition, home-furnishings retail, 2024
- **Source:** [Factoring Freight in Home Furnishings Retail](https://www.storis.com/?p=35117) — STORIS (furniture ERP vendor), 2024-05-05 (updated 2024-12-12)
- **Confidence:** high (vendor education page, matches generic definitions)
- **Use:** layer1-spec

### F-pricing-02 — Freight is estimated at PO time, then replaced with actuals and allocated to items by cost share (most common), cube, or weight
- **Value:** Practice description, 2024
- **Source:** [Factoring Freight in Home Furnishings Retail](https://www.storis.com/?p=35117) — STORIS, 2024
- **Confidence:** high
- **Use:** layer1-spec

### F-pricing-03 — Imported upholstered furniture carries a 25% Section 232 tariff since Oct 2025; the scheduled rise to 30% was postponed to 2027
- **Value:** 25% (upholstered furniture), 25% (kitchen cabinets/vanities, scheduled 50%), effective 2025-10-14; increases delayed 2025-12-31 to 2027
- **Source:** [Trump's furniture and cabinet tariffs take shape](https://businessofhome.com/articles/trump-s-furniture-and-cabinet-tariffs-take-shape) — Business of Home, 2025-09-30; [Furniture, cabinet tariff hikes delayed](https://www.retaildive.com/news/furniture-cabinets-tariffs-delay-trump-administration/808704/) — Retail Dive, 2025-12-31
- **Confidence:** high for the rates; medium for current status (last checked Dec 2025 coverage)
- **Use:** layer1-spec | submission-research

### F-pricing-04 — Annual inventory carrying cost is commonly 15–35% of inventory value (capital, storage, service, risk)
- **Value:** 15–35%/yr; capital component alone 8–15%; 2025–2026 vendor articles
- **Source:** [Calculate inventory carrying costs](https://www.cleverence.com/amp/articles/for-business/calculate-inventory-carrying-costs-4827/) — Cleverence (inventory software vendor), n.d. (2025–26)
- **Confidence:** medium (vendor blog; range is consistent with textbook rules of thumb, no furniture-specific figure found)
- **Use:** layer1-spec

### Layer 2 — Initial markup

### F-pricing-05 — "Keystone" is a 2.0x cost multiple; retailers' real initial markups range from "cost x2 plus $1–2" to multipliers of 2.2–2.3, and IMU must cover net profit + operating expense + markdowns
- **Value:** 2.0x–2.3x (general specialty retail), 2011
- **Source:** [Going Up?](https://lgrmag.com/?p=13814) — Paul Erickson, Lawn & Garden Retailer, Feb 2011
- **Confidence:** medium (not furniture-specific; the IMU formula is standard retail math)
- **Use:** layer1-spec

### F-pricing-06 — Share of furniture stores using exactly a 2.0x markup: 46% on queen bedding, 40% on master bedroom groups, 39% on leather stationary sofas; on mattresses 17% mark up above 2.0x and 37% below
- **Value:** Percent of surveyed stores, 2008 Furniture Store Performance Report
- **Source:** [Bedding's star still shines bright in furniture stores](https://www.furnituretoday.com/business-news/beddings-star-still-shines-bright-in-furniture-stores) — Furniture Today, 2008-10-13
- **Confidence:** medium (trade survey; dated)
- **Use:** layer1-spec | submission-research

### F-pricing-07 — Independent furniture store medians (2016): gross margin 46.5%, stock turns 4.0x, sales $200/sq ft of selling space, close ratio 22%
- **Value:** 46.5% GM (≈1.87x realized multiple), 2016
- **Source:** [Close ratios and stock turns decrease; gross margin increases](https://www.furnituretoday.com/business-news/close-ratios-and-stock-turns-decrease-gross-margin-increases) — Furniture Today, 2016-11-29
- **Confidence:** high for the survey year; medium as a 2026 benchmark (newer editions exist behind paywall; see Gaps)
- **Use:** layer1-spec | video-opener

### F-pricing-08 — Independent furniture store medians (2010): gross margin 47%, turns 3.2x, $160/sq ft, close ratio 35%, average transaction $875
- **Value:** 2010 Furniture Store Performance Report medians
- **Source:** [A peek inside furniture store operations](https://www.furnituretoday.com/business-news/a-peek-inside-furniture-store-operations) — Furniture Today, 2010-09-23
- **Confidence:** high (survey year), dated
- **Use:** submission-research

### F-pricing-09 — Havertys (public mid/upper chain) gross margin 60.7% in 2024 and 2023; occupancy and home-delivery costs sit in SG&A (58.0% of sales), not COGS
- **Value:** 60.7% GM ≈ 2.54x cost; SG&A 58.0%, FY2024
- **Source:** [Haverty Furniture Companies 10-K FY2024](https://www.sec.gov/Archives/edgar/data/216085/000162828025010869/hvt-20241231.htm) — SEC EDGAR, 2025
- **Confidence:** high
- **Use:** layer1-spec | pitch

### F-pricing-10 — Category gross-margin medians (2002): area rugs 47%, bedding 45%, casual dining 45%, stationary upholstery 45%; bedding GMROI $4.91 and turns 6.0 (highest)
- **Value:** 2002 Furniture Store Performance Report
- **Source:** [Bedding again leads list of high-profit products](https://www.furnituretoday.com/business-news/bedding-again-leads-list-of-high-profit-products) — Furniture Today, 2002-10-07
- **Confidence:** medium (very dated; only category-level split found)
- **Use:** layer1-spec

### Layer 3 — Vendor pricing policies

### F-pricing-11 — MAP sets the lowest advertised price; the store may still sell below it in person (example: $199 MSRP, $149 MAP, $119 in-store sale). Enforcement is loss of co-op funds or supply. Not all furniture vendors use MAP
- **Value:** Policy mechanics, 2018 (legal framing reconfirmed 2025)
- **Source:** [What should the furniture industry do about minimum advertised pricing?](https://www.furnituretoday.com/business-news/what-should-furniture-industry-minimum-advertised-pricing) — Furniture Today, 2018-06-18; [Minimum Advertised Price Policies: What Manufacturers Need to Know](https://www.foley.com/p/102kzwf/minimum-advertised-price-policies-what-manufacturers-need-to-know) — Foley & Lardner, Aug 2025
- **Confidence:** high
- **Use:** layer1-spec

### F-pricing-12 — Tempur-Pedic's retail pricing policy is a unilateral minimum resale price: it suspends shipments to retailers who sell below set prices; New York's challenge failed (2012), confirming such unilateral policies are lawful
- **Value:** Policy binds selling price, not just advertising; 2010–2012
- **Source:** [New York AG sues Tempur-Pedic over minimum pricing](https://www.furnituretoday.com/business-news/new-york-ag-sues-tempur-pedic-over-minimum-pricing) — Furniture Today, 2010-04-01; [People v. Tempur-Pedic, App. Div. 1st Dept.](https://www.nycourts.gov/reporter/3dseries/2012/2012_03557.htm) — NY Courts, 2012-05-08
- **Confidence:** high for 2010–12; medium that the policy is unchanged today (no 2023–25 source found)
- **Use:** layer1-spec

### F-pricing-13 — Ekornes (Stressless) polices "minimum retail price (MRP) guidelines" through selective distribution (~700 US storefronts)
- **Value:** Stressless chairs retailed $799–$2,199 at the time; 2002
- **Source:** [Ekornes eyes U.S. growth](https://www.furnituretoday.com/business-news/ekornes-eyes-us-growth) — Furniture Today, 2002-06-03
- **Confidence:** low as a current fact (very dated; no current public policy text found)
- **Use:** layer1-spec

### Layer 4 — Brand tier and construction

### F-pricing-14 — Eight-way hand-tied springs are "usually the most expensive option"; sinuous springs are mid-priced and "typically cost significantly less"; price alone does not reveal suspension type
- **Value:** Qualitative ordering; retailer education pages, 2024–26
- **Source:** [8-Way Hand-Tied Springs vs. Sinuous Springs](https://thisvsthat.io/8-way-hand-tied-springs-vs-sinuous-springs) — ThisVsThat, n.d.; [What's an 8-way hand-tied suspension?](https://rogerandchris.com/blog/260/whats-an-8-way-hand-tied-suspension) — Roger + Chris, n.d.
- **Confidence:** medium (no dollar delta found)
- **Use:** layer1-spec

### F-pricing-15 — Leather upholstery runs roughly 30% more than fabric on comparable pieces; a sectional uses 2–4x the hide of a sofa; bonded leather is ~17% leather and priced "a fraction" of top-grain (one seller claims 3–4x gap)
- **Value:** +30% leather vs fabric (dealer lineup); 3–4x bonded vs top-grain (seller claim), 2025–26
- **Source:** [How Much Does Leather Furniture Actually Cost?](https://furnitureacademy.com/how-much-does-leather-furniture-cost/) — Furniture Academy (dealer blog), 2026-06-11; [Bonded Leather Sofas Vs. Genuine Leather](https://www.servicemasterclean.com/blog/bonded-leather-sofas-vs-genuine-leather-price-durability-cleaning) — ServiceMaster Clean, n.d.; [Leather theater seating: top grain vs bonded vs faux](https://us.valenciatheaterseating.com/blogs/home-theater-seating/leather-theater-seating-top-grain-vs-bonded-vs-faux-what-actually-lasts) — Valencia (seller), n.d.
- **Confidence:** low–medium (single-dealer figures; vendor marketing)
- **Use:** layer1-spec

### F-pricing-16 — Veneer-over-engineered-core case goods can look near-identical to solid wood and cost about half; solid wood commands the premium for refinishability and material
- **Value:** ~50% price example ("oak finish" vs solid oak table), retailer page, n.d.
- **Source:** [Solid Wood vs. Veneer Wood: Which Is Better?](https://gphomefurniture.ca/blogs/news/solid-wood-vs-veneer-wood-which-is-better) — GP Home Furniture, n.d.
- **Confidence:** low (single retailer example)
- **Use:** layer1-spec

### Layer 5 — Material and color

### F-pricing-17 — No quantitative sell-through or markdown data by color was found; trade press records retailer anecdotes only (grays/neutrals as core; bold colors as accents; buyers reluctant to stock strong colors)
- **Value:** Qualitative, 2013 trade report
- **Source:** [Wider array of colors reaching retail floors](https://www.furnituretoday.com/business-news/wider-array-of-colors-reaching-retail-floors) — Furniture Today, 2013-06-05
- **Confidence:** medium that the evidence gap is real; low for any directional rule
- **Use:** layer1-spec

### F-pricing-18 — A single retailer reported a 595% increase in yellow-sofa sales over six months (UK, DFS) — a fashion-color spike, with no follow-up on later markdowns
- **Value:** +595%, Dec 2017–May 2018, UK
- **Source:** [We can't get enough of sunshine yellow sofas this summer](https://www.idealhome.co.uk/news/dfs-yellow-sofa-206391) — Ideal Home, 2018
- **Confidence:** low (company-reported, single retailer, UK)
- **Use:** submission-research

### Layer 6 — Trend signals

### F-pricing-19 — Pinterest Predicts 2026 is built from 600M monthly users' searches (Sep 2024–Aug 2025 vs prior year) and names furniture-relevant directions (Neo Deco, FunHaus stripes, Afrohemian); it reports search-growth percentages, not sales
- **Value:** Method and trend list, Dec 2025
- **Source:** [Pinterest Predicts 2026](https://www.apartmenttherapy.com/pinterest-predicts-2026-37522611) — Apartment Therapy, Dec 2025
- **Confidence:** high for method; trend-to-sales link unmeasured
- **Use:** layer1-spec

### F-pricing-20 — Google Trends predicts retail sales in aggregate (up to three quarters ahead in one study) but is a 0–100 relative index with a privacy threshold and sampling noise; small regions and low-volume terms return zeros or unstable values
- **Value:** Method limits, 2019–2025
- **Source:** [Forecasting retail sales just got smarter thanks to Google searches](https://www.business.rice.edu/wisdom/forecasting-retail-sales-just-got-smarter-thanks-google-searches) — Rice Business; [Where you are is what you get? Sample inconsistencies of Google Trends data](https://www.mzes.uni-mannheim.de/en/publications/details/default-1b90339871013c563d9e0770aa21fed2-44) — MZES Mannheim; [Google Trends not working / zeros](https://meetglimpse.com/google-trends/not-working/) — Glimpse
- **Confidence:** high
- **Use:** layer1-spec

### F-pricing-21 — Vendor introduction calendar: High Point Market Apr 25–29 and Oct 17–21, 2026; Las Vegas Market Jan 25–29 and Jul 26–30, 2026
- **Value:** Dates, 2026
- **Source:** [AHFA non-AHFA events 2026](https://ahfa.us/events/nonahfa/2026) — AHFA; [Las Vegas Market Winter 2026 returns](https://www.giftsanddec.com/las-vegas-market-furniture-show/las-vegas-market-winter-2026-returns-with-fresh-offerings) — Gifts & Decorative Accessories, 2025-12-23
- **Confidence:** high
- **Use:** layer1-spec

### F-pricing-22 — 46% of furniture shoppers research online before buying in store; 45% shop both channels
- **Value:** 46%, 45%, 2025 (3D Cloud / Provoke Insights study)
- **Source:** [Digital tools reshape furniture shopping trends](https://www.interiordaily.com/article/9712116/digital-tools-reshape-furniture-shopping-trends/) — Interior Daily, 2025-03-10
- **Confidence:** medium (vendor-sponsored survey; sample size not stated in article)
- **Use:** layer1-spec | pitch

### F-pricing-23 — 60% of US adults who bought furniture in the past year felt they paid above an acceptable price (sofas 62%, dining tables 66%, mattresses 61%); 83% would trade down
- **Value:** 60% / 62% / 66% / 61% / 83%, n=2,000, summer 2025
- **Source:** [Furniture shoppers are trading down, survey finds](https://www.designerstoday.com/furniture/side-effect-of-tariff-fatigue-furniture-shoppers-are-trading-down-survey-finds) — Designers Today citing L.E.K. Consulting, 2025-10-15
- **Confidence:** high
- **Use:** video-opener | pitch

### Layer 7 — Age and velocity

### F-pricing-24 — GMROI = gross margin dollars ÷ average inventory at cost; furniture benchmark bands quoted as 1.3–2.5 (one source) and 2.0–3.0 (others)
- **Value:** 1.3–2.5 (eightx); "around 2.0–2.5" (Toolio); $2–3 home goods (SPS Commerce); 2025–26
- **Source:** [What is GMROI](https://eightx.co/blog/what-is-gmroi) — Eightx, 2026-06-01; [The Complete Guide to GMROI](https://www.toolio.com/post/the-complete-guide-to-gmroi-for-retail-brands) — Toolio
- **Confidence:** medium (consultant/vendor benchmarks disagree)
- **Use:** layer1-spec

### F-pricing-25 — Sell-through = units sold ÷ units received in a period; home goods & furnishings guideline 15–40% monthly "or lower due to higher price and consideration time"
- **Value:** 15–40%/month, 2026
- **Source:** [Sell-Through Rate Benchmarks By Category](https://racklify.com/encyclopedia/sell-through-rate-benchmarks-by-category-what-good-looks-like-for-retailers/) — Racklify, 2026-09-17
- **Confidence:** medium (encyclopedia-style vendor content)
- **Use:** layer1-spec

### F-pricing-26 — General-retail aged-inventory playbooks step actions at ~90, 180, and 270–365 days (e.g., 20% off at 91–180 days, outlet transfer at 181–270, liquidate past 270); common aging buckets are 0–30/31–60/61–90/91–120/120+ days. No furniture-specific published cadence found
- **Value:** Day thresholds and example discounts, 2026
- **Source:** [How Warehouse Managers Should Handle Aged Inventory](https://racklify.com/encyclopedia/how-warehouse-managers-should-handle-aged-inventory-strategies-for-reduction/) — Racklify, 2026; [10 Inventory Aging Reports Every Retailer Needs](https://www.increff.com/blog/10-inventory-aging-reports-every-retailer-needs) — Increff, 2026-08-31
- **Confidence:** medium for the buckets; low that these discount depths apply to furniture
- **Use:** layer1-spec

### F-pricing-27 — Floor-model discounts: no standard; most 10–15%, up to ~40% for worn or long-displayed units; Costco floor models start ~10% off
- **Value:** 10–15% typical, up to 40%, 2024–26
- **Source:** [What Are Floor Model Appliances and Should You Buy One?](https://www.homeserve.com/blog/buying-guide/floor-model-appliances) — HomeServe; [Costco floor-model furniture discounts](https://www.moneydigest.com/1841896/costco-discount-floor-model-big-savings-on-furniture/) — Money Digest
- **Confidence:** low–medium (consumer blogs; appliance-leaning)
- **Use:** layer1-spec

### F-pricing-28 — Independent-store median stock turns fell from 4.3x (2015) to 4.0x (2016); a 2025 planning guide treats 2.0–3.0x as workable and below 1.8x as weak
- **Value:** 4.0x median (2016); 2.0–3.0x target (2025 guide)
- **Source:** [Close ratios and stock turns decrease](https://www.furnituretoday.com/business-news/close-ratios-and-stock-turns-decrease-gross-margin-increases) — Furniture Today, 2016-11-29; [Furniture Store Business Idea Overview](https://startupfinancialprojection.com/blogs/profitability/furniture-store) — StartupFinancialProjection, 2025 (page returned 410 on re-fetch; figures from search index)
- **Confidence:** high / low respectively
- **Use:** layer1-spec

### Layer 8 — Scarcity and lead time

### F-pricing-29 — Current custom-upholstery lead times: Four Hands 8–10 weeks (Sep 2025); Flexsteel domestic made-to-order 4 weeks (2022); typical branded upholstery 12–16 weeks and peak-2022 extremes of 35–51 weeks
- **Value:** 8–10 wk; 4 wk; 12–16 wk; 35–51 wk peak, 2022–2025
- **Source:** [Four Hands launches custom upholstery program with faster lead times](https://www.furnituretoday.com/tag/lead-times) — Furniture Today, 2025-09-25; [Is the lead time crisis almost over?](https://businessofhome.com/articles/is-the-lead-time-crisis-almost-over) — Business of Home, 2022-08-17
- **Confidence:** high for the cited brands; medium as a general 2026 range (the owner's 14-week example, A-S029–032, is inside it)
- **Use:** layer1-spec

### F-pricing-30 — Special orders typically require a deposit and are non-returnable, which is why stores discount them less than stock
- **Value:** Policy pattern (La-Z-Boy store listing: "Downpayment required", "No returns" on special orders)
- **Source:** [La-Z-Boy Home Furnishings & Decor — Checkbook listing](https://www.checkbook.org/wa/tukwila/furniture-stores/la-z-boy-home-furnishings-and-decor/di5eh) — Consumers' Checkbook
- **Confidence:** low (single store listing; the pricing inference is ours)
- **Use:** layer1-spec

### Layer 9 — Seasonal and event pricing

### F-pricing-31 — Black Friday 2024: furniture discounts averaged 36% across 4,300+ ads from 13 big retailers (Macy's ~53%, Walmart 50%, Target 43%, Home Depot 41%, Amazon 25%, Costco 24%); furniture was ~4% of all deals
- **Value:** 36% average, 2024
- **Source:** [Major retailers are rolling out Black Friday furniture deals, ad analysis shows](https://www.furnituretoday.com/?p=323376) — Furniture Today citing WalletHub, 2024-11-20
- **Confidence:** high (ad analysis, not realized prices)
- **Use:** layer1-spec | submission-research

### F-pricing-32 — Holiday-weekend furniture promotions (Memorial Day, Labor Day, Veterans Day) run 20–30% off; mattresses 50–80% off reference price on holiday weekends; January–February and July–August are the clearance windows before new introductions
- **Value:** 20–30% (furniture), 50–80% (mattress reference discounts), 2014–2024
- **Source:** [7 Questions to Ask Before You Buy a Couch](https://oprah.com/home/couch-tips-buying-a-sofa/5) — Oprah.com, 2014; [Best Times to Buy Furniture](https://kiplinger.com/article/spending/t050-c011-s001-best-times-to-buy-furniture-when-redecorating.html) — Kiplinger (Offers.com CEO estimate); [Best time to buy furniture](https://lugg.com/blog/best-time-to-buy-furniture) — Lugg
- **Confidence:** low–medium (consumer press; Kiplinger page truncated on fetch)
- **Use:** layer1-spec

### F-pricing-33 — "Up to X% off" events are legal only if enough items actually carry the maximum; FTC and self-regulatory guidance differ and no numeric threshold is published
- **Value:** Rule of practice, 2025
- **Source:** [In honor of Prime Day: a primer on advertising sales](https://advertisinglaw.fkks.com/post/102gi39/in-honor-of-prime-day-a-primer-on-advertising-sales) — Frankfurt Kurnit (advertising law blog)
- **Confidence:** medium
- **Use:** layer1-spec

### Layer 10 — Competitors and online comparables

### F-pricing-34 — Ashley price-matches only identical in-stock items "sold and fulfilled" by five or six named online sellers (Amazon, Wayfair, Overstock, Target, Hayneedle, later Walmart); La-Z-Boy matches stores within 50 miles
- **Value:** Policy terms, 2019–2025
- **Source:** [Ashley Furniture's Price Match Policy](https://www.truthinadvertising.org/ashley-furnitures-price-match-policy/) — Truth in Advertising; [Does La-Z-Boy Price Match?](https://furnitureacademy.com/does-la-z-boy-price-match/) — Furniture Academy
- **Confidence:** medium (terms change; verify current pages)
- **Use:** layer1-spec

### F-pricing-35 — Brick-and-mortar retailers treat MAP as protection against online discounters and lean on service: a Dallas independent offers white-glove delivery within 500 miles; online sellers evade MAP with in-cart pricing
- **Value:** Qualitative, 2018
- **Source:** [What should the furniture industry do about MAP?](https://www.furnituretoday.com/business-news/what-should-furniture-industry-minimum-advertised-pricing) — Furniture Today, 2018-06-18
- **Confidence:** high
- **Use:** layer1-spec | pitch

### F-pricing-36 — White-glove delivery is priced $150–$500+ per stop by third-party carriers versus $15–$50 for standard drop-off; retailer fees cluster around $99–$149 per order
- **Value:** $150–500/stop (3PL guide); $149 under $1,500 orders (Portland store), 2025–26
- **Source:** [White glove delivery guide](https://www.wearewarp.com/warp-blogs/white-glove-delivery-guide) — Warp (3PL), 2026 (per-stop figures appeared in search excerpt; page body on fetch showed service description only); [Delivery & Shipping FAQ](https://whatsnewfurniture.com/pages/delivery-faq) — What's New Furniture
- **Confidence:** low (unconfirmed on page; use owner's actual crew cost instead)
- **Use:** layer1-spec

### Layer 11 — Negotiation and concessions

### F-pricing-37 — 48% of Americans tried haggling in the prior three years (down from 61% in 2007); 89% of hagglers succeeded; furniture hagglers saved $300 on average; 57% used "I'll check competitors' prices"
- **Value:** 48%, 89%, $300, 57%; n=2,000, 2013
- **Source:** [Consumer Reports' Survey: Nine of 10 Americans Who Haggled Saved Money](https://www.consumerreports.org/media-room/press-releases/2013/07/my-entry) — Consumer Reports, 2013-07-10
- **Confidence:** high for 2013; dated
- **Use:** video-opener | submission-research

### F-pricing-38 — Haggling is more common at independent retailers than chains because owners and managers have more leeway; chains keep official no-haggle policies but adjust on one-of-a-kind and clearance items
- **Value:** Qualitative, 2008 consumer-behavior firm finding
- **Source:** [Haggling making a comeback](https://honoluluadvertiser.com/article/2008/May/11/bz/hawaii805110345.html) — Honolulu Advertiser, 2008-05-11; [The Secret National Retailers Don't Want You to Know About](https://business.time.com/?p=3297) — TIME
- **Confidence:** low–medium (dated, secondary)
- **Use:** pitch

### F-pricing-39 — Tiered discount authority is the standard control: rep alone up to ~10%, manager 10–25%, executive above; POS systems enforce it with manager PIN overrides
- **Value:** Example tiers (10% / 25%), 2025–26
- **Source:** [Discount approval](https://dealhub.io/glossary/discount-approval/) — DealHub glossary; [Manager approval (POS)](https://docs.infor.com/shub/2024.x/en-us/shubrg/uym1540990657049.html) — Infor docs, 2024
- **Confidence:** medium (generic B2B/retail; no furniture-specific tiers published)
- **Use:** layer1-spec

### F-pricing-40 — Furniture sales commissions are paid on "written" (deposit taken) or "delivered" sales; one current posting pays 7% of written sales. No industry benchmark table found
- **Value:** 7% on written sales (EQ3 design consultant posting), 2025–26
- **Source:** [Design Consultant at EQ3](https://designproject.io/jobs/design-consultant-at-eq3-czidob) — Design Project job board; [Furniture retail glossary: written vs delivered](https://pay.bestbuy-furniture.com/blog/furniture-retail-glossary)
- **Confidence:** low (single posting; the owner's 6% figure, B-S125–144, is plausible but unverified)
- **Use:** layer1-spec

### Layer 12 — Floor-space cost (for clearance reasoning)

### F-pricing-41 — California metro retail asking rents: Bay Area $33.18/sq ft/yr NNN (Q1 2025); Los Angeles $36.50/sq ft/yr (Q3 2025); San Francisco $43.75 (Q2 2026); Fresno $19.60 (Q4 2025)
- **Value:** $19.60–$43.75 per sq ft per year, 2025–26
- **Source:** [Bay Area Retail Figures Q1 2025](https://www.cbre.com/insights/figures/bay-area-retail-figures-q1-2025) — CBRE; [Los Angeles Retail Market Report Q3 2025](https://www.matthews.com/insights/los-angeles-retail-market-report-q325) — Matthews; [2026 Q2 San Francisco Retail](https://www.lee-associates.com/wp-content/uploads/2026/07/2026-Q2-San-Francisco-CA-Retail.pdf) and [2025 Q4 Fresno Retail](https://www.lee-associates.com/wp-content/uploads/2026/01/2025-Q4-Fresno-CA-Retail.pdf) — Lee & Associates
- **Confidence:** high (broker averages; the store's own lease governs)
- **Use:** layer1-spec

### Layer 13 — Legal guardrail

### F-pricing-42 — FTC 16 CFR 233.1: a former price is legitimate only if it was "the actual, bona fide price at which the article was offered to the public on a regular basis" for a reasonably substantial period; an inflated price set up to enable a later "discount" is fictitious; do not imply it was a selling price unless substantial sales were made at it
- **Value:** Federal guide text (advisory, enforced via FTC Act §5 and state UDAP laws)
- **Source:** [16 CFR § 233.1 Former price comparisons](https://www.law.cornell.edu/cfr/text/16/233.1) — Cornell LII
- **Confidence:** high
- **Use:** layer1-spec

### F-pricing-43 — FTC 16 CFR 233.2–233.3: comparisons to competitors or to MSRP/list are deceptive unless the higher price does not appreciably exceed what principal outlets in the trade area actually charge for substantial sales
- **Value:** Federal guide text
- **Source:** [16 CFR § 233.2](https://www.law.cornell.edu/cfr/text/16/233.2) and [16 CFR § 233.3](https://www.law.cornell.edu/cfr/text/16/233.3) — Cornell LII
- **Confidence:** high
- **Use:** layer1-spec

### F-pricing-44 — California B&P §17501: a "former price" may be advertised only if it was the prevailing market price in the locality within the three months before the ad, or the date it prevailed is stated "clearly, exactly and conspicuously"; 4 CCR §1302 repeats this; Civil Code §1770(a)(13) bans false statements about "reasons for, existence of, or amounts of, price reductions"; an appellate court upheld §17501 against a vagueness challenge in 2019
- **Value:** Three-month rule; statutes current
- **Source:** [Cal. Bus. & Prof. Code § 17501](https://codes.findlaw.com/ca/business-and-professions-code/bpc-sect-17501/) — FindLaw; [4 CCR § 1302](https://regulations.justia.com/states/california/title-4/division-3/article-10/section-1302) — Justia; [Cal. Civ. Code § 1770](https://codes.findlaw.com/ca/civil-code/civ-sect-1770/) — FindLaw; [California Appellate Panel Upholds Validity of Pricing Statute](https://www.manatt.com/insights/newsletters/advertising-law/california-appellate-panel-upholds-validity-of-pri) — Manatt, 2019
- **Confidence:** high
- **Use:** layer1-spec

## Tables

### Master table — inputs, direction of effect, measurability

Direction key: ↑ raises, ↓ lowers, → sets/bounds, ~ small or indirect, ? unmeasured.

| Layer | Input field needed | Direction of effect on tag price | Direction of effect on floor | Measurable by a small store today? | Source IDs |
|---|---|---|---|---|---|
| 1 Cost basis | Vendor invoice cost per unit | → base of multiple | → hard lower bound | yes (invoice) | F-01 |
| 1 Cost basis | Inbound freight allocated per item (cost-share, cube, or weight) | ↑ (adds to landed) | ↑ | yes if freight bills are kept; partly if estimated | F-01, F-02 |
| 1 Cost basis | Duties/tariffs (25% on imported upholstery since Oct 2025) | ↑ | ↑ | yes (on invoice or customs line) | F-03 |
| 1 Cost basis | Receiving/prep/deluxing labor | ↑ ~ | ↑ ~ | partly (usually not tracked per item) | F-01 |
| 1 Cost basis | Outbound delivery cost per stop (own crew) | ~ (often priced separately) | ↑ when delivery is "free" in the deal | partly (crew payroll ÷ stops) | F-36, F-09 |
| 1 Cost basis | Holding cost (15–35%/yr of cost) × months on floor | ~ | ↓ willingness to hold out as age grows | yes (receipt date + rate assumption) | F-04 |
| 2 Markup | Category (upholstery, case goods, bedding, rugs, accents) | → sets multiple (keystone anchor; bedding/rugs highest GM) | ~ | yes | F-05, F-06, F-10 |
| 2 Markup | Store's target gross margin (46–47% indie median; 60.7% chain) | → | → (floor = cost ÷ (1 − min GM)) | yes (owner decision) | F-07, F-08, F-09 |
| 2 Markup | Planned markdown allowance in IMU | ↑ tag to fund later promos | ~ | partly | F-05 |
| 3 Vendor policy | MAP price (per SKU) | → minimum *advertised* tag | none (in-store sale below MAP legal) | yes if vendor supplies MAP list | F-11, F-35 |
| 3 Vendor policy | Unilateral minimum retail price (Tempur-Pedic, Stressless/Ekornes) | → tag ≥ UMRP | → floor ≥ UMRP (supply cut-off risk) | yes for those brands; policy text not public | F-12, F-13 |
| 4 Brand tier | Brand positioning (promotional/mid/better/best) | ↑ with tier | ↑ (less discount expected) | yes (owner tags) | F-14–F-16 |
| 4 Construction | Suspension (8-way hand-tied > sinuous), frame (kiln-dried hardwood) | ↑ | ↑ | yes (spec sheet) | F-14 |
| 4 Construction | Cover (top-grain/full-grain > fabric ≈ +30% > bonded) | ↑ | ↑ | yes | F-15 |
| 4 Construction | Solid wood vs veneer case goods | ↑ (~2x example) | ↑ | yes | F-16 |
| 5 Color/finish | Neutral vs fashion color | ? (no sell-through data) | ↓ for fashion colors only via age (slower sell-through) | partly (own sales history by color) | F-17, F-18 |
| 6 Trend | Google Trends index for item/style terms | ~ ↑ when rising | ~ | partly (state-level only; noisy below) | F-20 |
| 6 Trend | Pinterest Predicts / market introductions (HP Apr/Oct, LV Jan/Jul) | ~ ↑ for trend-right; ↓ for outgoing styles after market | ↓ for soon-to-be-discontinued | yes (calendar), partly (relevance) | F-19, F-21 |
| 6 Trend | Local sell-through of the SKU/style (units sold ÷ received) | ↑ if fast | ↑ if fast (don't discount a seller) | yes (POS or ledger) | F-25 |
| 7 Age | Days since receipt (buckets 90/180/270–365) | ↓ via markdown schedule | ↓ stepwise | yes (receipt date) | F-26, F-04 |
| 7 Age | Floor model / wear condition | ↓ 10–15% typical, to ~40% | ↓ | yes | F-27 |
| 7 Velocity | Category turns and GMROI vs benchmark (turns ~4x median; GMROI 1.3–2.5) | ~ | ↓ for items dragging GMROI | yes with annual COGS and avg inventory | F-24, F-28 |
| 7 Space | Rent per sq ft × footprint × months ($33–37/sf/yr CA metro) | ~ | ↓ (quantified cost of keeping it) | yes (lease ÷ floor sq ft) | F-41 |
| 8 Scarcity | Discontinued / last unit | ↓ tag if clearing; ↑ if unique | ↑ if sought-after, ↓ if orphaned | yes (vendor notice) | F-30, F-29 |
| 8 Lead time | Special-order lead time (8–16 wk typical) and reorderability | ↑ for in-stock premium vs 12-week wait | ↑ (in-stock availability is the service argument) | yes (vendor quote) | F-29, F-30 |
| 8 Terms | Special order = deposit, no returns | ~ | ↑ (little reason to discount a made-to-order piece) | yes | F-30 |
| 9 Season | Promo calendar (Presidents, Memorial, July 4, Labor, Black Friday, year-end) | ↓ 20–36% event depth | ↓ temporarily; must still clear floor | yes | F-31, F-32 |
| 9 Event build | "Up to X%" item-level assignment (bigger on aged, smaller on sellers) | ↓ varies by item | ↓ varies | yes | F-33, F-26 |
| 10 Competitors | Online comparable price (Wayfair/Amazon/Ashley) for identical SKU | → ceiling for identical goods | ↓ pressure; offset by service | partly (manual lookup; MAP-hidden prices) | F-22, F-34 |
| 10 Service | Delivery/white-glove/availability bundle | ↑ justifies premium | ↑ (concession has a cost) | yes | F-35, F-36 |
| 11 Negotiation | Expected haggle rate and average concession (~$300 CR 2013) | ↑ tag to leave room | → floor set below tag by expected concession | partly (own deal history) | F-37, F-38, F-23 |
| 11 Authority | Discount tiers (rep ≤10%, manager ≤25%, owner above) | none | → who may approach the floor | yes (owner policy) | F-39 |
| 11 Incentive | Commission basis (written vs delivered; % of sale vs margin) | none | ↓ pressure from sales staff | yes | F-40 |
| 12 Legal | Former-price history (date, duration, sales at that price) | → tag must be a real, offered price before it can be a "was" price | none | yes (price-change log) | F-42, F-44 |
| 12 Legal | MSRP/competitor reference validity in trade area | → "compare at" only if principal outlets charge it | none | partly | F-43 |

Rows: 35.

### What a tool must not do (legal)

| Prohibited | Rule |
|---|---|
| Raise a tag to $300, strike it, and sell at the unchanged $200 as a "sale" | 16 CFR 233.1 (fictitious former price); Cal. B&P §17501 (not the prevailing price in prior 3 months); Civ. Code §1770(a)(13) |
| Show a "was" price older than 3 months without the date it prevailed | Cal. B&P §17501; 4 CCR §1302 |
| Print "MSRP $X" or "compare at $X" when no principal local outlet sells at X | 16 CFR 233.3, 233.2 |
| Advertise "up to 50% off" when only a token item is at 50% | 16 CFR 233 practice; state UDAP |
| Advertise below MAP, or sell below a vendor's unilateral minimum retail price | Vendor policy (supply cut-off), not law |
| Record a negotiated price as a "discount from regular" when the regular price never held | 233.1(b); §17501 |

## Gaps and unverified

- Vendor-specific MAP/UMRP terms for La-Z-Boy, Flexsteel, Hooker, Bassett, and Ashley: not found on any public vendor or trade-press page; these live in dealer agreements. Tempur-Pedic (2010–12 litigation) and Ekornes (2002 trade article) are the only sourced cases. Treat "brand X enforces MAP" as an owner-entered field, not a fact.
- Current Furniture Today Furniture Store Performance Report (2024/2025 editions exist; paywalled). Latest open medians are 2016 (GM 46.5%, turns 4.0x, $200/sq ft). Category markup multiples beyond the 2008 "share using 2.0x" data: not found.
- Color: no dataset relating color/finish to sell-through or markdown depth in furniture. Yanko Design's "pink loses 60–70% on resale" and "returns up 300%" claims cite no source and are excluded. Estimate only.
- Furniture-specific aging-to-markdown cadence (90/180/365): not published; the thresholds cited are general retail and warehouse practice.
- Haggling data is 2013 (Consumer Reports); the "87% success rate for furniture" figure appears only in secondary TV write-ups, not in the CR press release, so it is omitted.
- Delivery expense as % of sales and "delivery income offsets 60–75% of delivery expense" (Home Furnishings Business) — page would not load; unverified.
- Per-stop white-glove pricing ($150–500) appeared in a search excerpt of the Warp page but not in the fetched page body; low confidence.
- Commission norms: one 7% posting; no industry table. Owner's 6% is plausible, unverified.
- Discount-authority tiers in furniture specifically: not published; tiers shown are generic sales-ops practice.
- Kiplinger and Baer's pages returned truncated/403; their claims are carried at low confidence or omitted.
- Numbers that are estimates, not measurements: carrying-cost %, GMROI bands, floor-model discount ranges, holiday discount depths (ad-analysis, not transaction prices).

## Sources

1. Factoring Freight in Home Furnishings Retail — STORIS, 2024-05-05 — https://www.storis.com/?p=35117
2. Trump's furniture and cabinet tariffs take shape — Business of Home, 2025-09-30 — https://businessofhome.com/articles/trump-s-furniture-and-cabinet-tariffs-take-shape
3. Furniture, cabinet tariff hikes delayed — Retail Dive, 2025-12-31 — https://www.retaildive.com/news/furniture-cabinets-tariffs-delay-trump-administration/808704/
4. Calculate inventory carrying costs — Cleverence, n.d. — https://www.cleverence.com/amp/articles/for-business/calculate-inventory-carrying-costs-4827/
5. Going Up? — Lawn & Garden Retailer, Feb 2011 — https://lgrmag.com/?p=13814
6. Bedding's star still shines bright in furniture stores — Furniture Today, 2008-10-13 — https://www.furnituretoday.com/business-news/beddings-star-still-shines-bright-in-furniture-stores
7. Close ratios and stock turns decrease; gross margin increases — Furniture Today, 2016-11-29 — https://www.furnituretoday.com/business-news/close-ratios-and-stock-turns-decrease-gross-margin-increases
8. A peek inside furniture store operations — Furniture Today, 2010-09-23 — https://www.furnituretoday.com/business-news/a-peek-inside-furniture-store-operations
9. Haverty Furniture Companies 10-K FY2024 — SEC EDGAR, 2025 — https://www.sec.gov/Archives/edgar/data/216085/000162828025010869/hvt-20241231.htm
10. Bedding again leads list of high-profit products — Furniture Today, 2002-10-07 — https://www.furnituretoday.com/business-news/bedding-again-leads-list-of-high-profit-products
11. What should the furniture industry do about minimum advertised pricing? — Furniture Today, 2018-06-18 — https://www.furnituretoday.com/business-news/what-should-furniture-industry-minimum-advertised-pricing
12. Minimum Advertised Price Policies: What Manufacturers Need to Know — Foley & Lardner, Aug 2025 — https://www.foley.com/p/102kzwf/minimum-advertised-price-policies-what-manufacturers-need-to-know
13. New York AG sues Tempur-Pedic over minimum pricing — Furniture Today, 2010-04-01 — https://www.furnituretoday.com/business-news/new-york-ag-sues-tempur-pedic-over-minimum-pricing
14. People v. Tempur-Pedic International (App. Div. 1st Dept.) — NY Courts, 2012-05-08 — https://www.nycourts.gov/reporter/3dseries/2012/2012_03557.htm
15. Ekornes eyes U.S. growth — Furniture Today, 2002-06-03 — https://www.furnituretoday.com/business-news/ekornes-eyes-us-growth
16. 8-Way Hand-Tied Springs vs. Sinuous Springs — ThisVsThat, n.d. — https://thisvsthat.io/8-way-hand-tied-springs-vs-sinuous-springs
17. What's an 8-way hand-tied suspension? — Roger + Chris, n.d. — https://rogerandchris.com/blog/260/whats-an-8-way-hand-tied-suspension
18. How Much Does Leather Furniture Actually Cost? — Furniture Academy, 2026-06-11 — https://furnitureacademy.com/how-much-does-leather-furniture-cost/
19. Bonded Leather Sofas Vs. Genuine Leather — ServiceMaster Clean, n.d. — https://www.servicemasterclean.com/blog/bonded-leather-sofas-vs-genuine-leather-price-durability-cleaning
20. Leather theater seating: top grain vs bonded vs faux — Valencia Theater Seating, n.d. — https://us.valenciatheaterseating.com/blogs/home-theater-seating/leather-theater-seating-top-grain-vs-bonded-vs-faux-what-actually-lasts
21. Solid Wood vs. Veneer Wood — GP Home Furniture, n.d. — https://gphomefurniture.ca/blogs/news/solid-wood-vs-veneer-wood-which-is-better
22. Wider array of colors reaching retail floors — Furniture Today, 2013-06-05 — https://www.furnituretoday.com/business-news/wider-array-of-colors-reaching-retail-floors
23. We can't get enough of sunshine yellow sofas this summer — Ideal Home, 2018 — https://www.idealhome.co.uk/news/dfs-yellow-sofa-206391
24. Pinterest Predicts 2026 — Apartment Therapy, Dec 2025 — https://www.apartmenttherapy.com/pinterest-predicts-2026-37522611
25. Forecasting retail sales just got smarter thanks to Google searches — Rice Business — https://www.business.rice.edu/wisdom/forecasting-retail-sales-just-got-smarter-thanks-google-searches
26. Where you are is what you get? Sample inconsistencies of Google Trends data — MZES Mannheim — https://www.mzes.uni-mannheim.de/en/publications/details/default-1b90339871013c563d9e0770aa21fed2-44
27. Google Trends not working / zeros — Glimpse — https://meetglimpse.com/google-trends/not-working/
28. Non-AHFA events 2026 (High Point Market dates) — AHFA — https://ahfa.us/events/nonahfa/2026
29. Las Vegas Market Winter 2026 returns — Gifts & Decorative Accessories, 2025-12-23 — https://www.giftsanddec.com/las-vegas-market-furniture-show/las-vegas-market-winter-2026-returns-with-fresh-offerings
30. Digital tools reshape furniture shopping trends — Interior Daily, 2025-03-10 — https://www.interiordaily.com/article/9712116/digital-tools-reshape-furniture-shopping-trends/
31. Furniture shoppers are trading down, survey finds (L.E.K.) — Designers Today, 2025-10-15 — https://www.designerstoday.com/furniture/side-effect-of-tariff-fatigue-furniture-shoppers-are-trading-down-survey-finds
32. What is GMROI — Eightx, 2026-06-01 — https://eightx.co/blog/what-is-gmroi
33. The Complete Guide to GMROI — Toolio — https://www.toolio.com/post/the-complete-guide-to-gmroi-for-retail-brands
34. Sell-Through Rate Benchmarks By Category — Racklify, 2026-09-17 — https://racklify.com/encyclopedia/sell-through-rate-benchmarks-by-category-what-good-looks-like-for-retailers/
35. How Warehouse Managers Should Handle Aged Inventory — Racklify, 2026 — https://racklify.com/encyclopedia/how-warehouse-managers-should-handle-aged-inventory-strategies-for-reduction/
36. 10 Inventory Aging Reports Every Retailer Needs — Increff, 2026-08-31 — https://www.increff.com/blog/10-inventory-aging-reports-every-retailer-needs
37. What Are Floor Model Appliances and Should You Buy One? — HomeServe — https://www.homeserve.com/blog/buying-guide/floor-model-appliances
38. Costco floor-model furniture discounts — Money Digest — https://www.moneydigest.com/1841896/costco-discount-floor-model-big-savings-on-furniture/
39. Furniture Store Business Idea Overview — StartupFinancialProjection, 2025 (410 on re-fetch) — https://startupfinancialprojection.com/blogs/profitability/furniture-store
40. Lead times tag (Four Hands 8–10 weeks, Flexsteel 4 weeks) — Furniture Today, 2025-09-25 / 2022-06-14 — https://www.furnituretoday.com/tag/lead-times
41. Is the lead time crisis almost over? — Business of Home, 2022-08-17 — https://businessofhome.com/articles/is-the-lead-time-crisis-almost-over
42. La-Z-Boy Home Furnishings & Decor listing — Consumers' Checkbook — https://www.checkbook.org/wa/tukwila/furniture-stores/la-z-boy-home-furnishings-and-decor/di5eh
43. Major retailers are rolling out Black Friday furniture deals (WalletHub) — Furniture Today, 2024-11-20 — https://www.furnituretoday.com/?p=323376
44. 7 Questions to Ask Before You Buy a Couch — Oprah.com, 2014 — https://oprah.com/home/couch-tips-buying-a-sofa/5
45. Best Times to Buy Furniture — Kiplinger — https://kiplinger.com/article/spending/t050-c011-s001-best-times-to-buy-furniture-when-redecorating.html
46. Best time to buy furniture — Lugg — https://lugg.com/blog/best-time-to-buy-furniture
47. In honor of Prime Day: a primer on advertising sales — Frankfurt Kurnit — https://advertisinglaw.fkks.com/post/102gi39/in-honor-of-prime-day-a-primer-on-advertising-sales
48. Ashley Furniture's Price Match Policy — Truth in Advertising — https://www.truthinadvertising.org/ashley-furnitures-price-match-policy/
49. Does La-Z-Boy Price Match? — Furniture Academy — https://furnitureacademy.com/does-la-z-boy-price-match/
50. White glove delivery guide — Warp, 2026 — https://www.wearewarp.com/warp-blogs/white-glove-delivery-guide
51. Delivery & Shipping FAQ — What's New Furniture — https://whatsnewfurniture.com/pages/delivery-faq
52. Consumer Reports' Survey: Nine of 10 Americans Who Haggled Saved Money — Consumer Reports, 2013-07-10 — https://www.consumerreports.org/media-room/press-releases/2013/07/my-entry
53. Haggling making a comeback — Honolulu Advertiser, 2008-05-11 — https://honoluluadvertiser.com/article/2008/May/11/bz/hawaii805110345.html
54. The Secret National Retailers Don't Want You to Know About — TIME — https://business.time.com/?p=3297
55. Discount approval — DealHub glossary — https://dealhub.io/glossary/discount-approval/
56. Manager approval (POS discount override) — Infor docs, 2024 — https://docs.infor.com/shub/2024.x/en-us/shubrg/uym1540990657049.html
57. Design Consultant at EQ3 (7% on written sales) — Design Project — https://designproject.io/jobs/design-consultant-at-eq3-czidob
58. Furniture retail glossary (written vs delivered) — https://pay.bestbuy-furniture.com/blog/furniture-retail-glossary
59. Bay Area Retail Figures Q1 2025 — CBRE — https://www.cbre.com/insights/figures/bay-area-retail-figures-q1-2025
60. Los Angeles Retail Market Report Q3 2025 — Matthews — https://www.matthews.com/insights/los-angeles-retail-market-report-q325
61. 2026 Q2 San Francisco CA Retail — Lee & Associates — https://www.lee-associates.com/wp-content/uploads/2026/07/2026-Q2-San-Francisco-CA-Retail.pdf
62. 2025 Q4 Fresno CA Retail — Lee & Associates — https://www.lee-associates.com/wp-content/uploads/2026/01/2025-Q4-Fresno-CA-Retail.pdf
63. 16 CFR § 233.1 Former price comparisons — Cornell LII — https://www.law.cornell.edu/cfr/text/16/233.1
64. 16 CFR § 233.2 Retail price comparisons; comparable value comparisons — Cornell LII — https://www.law.cornell.edu/cfr/text/16/233.2
65. 16 CFR § 233.3 Advertising retail prices which have been established or suggested by manufacturers — Cornell LII — https://www.law.cornell.edu/cfr/text/16/233.3
66. Cal. Bus. & Prof. Code § 17501 — FindLaw — https://codes.findlaw.com/ca/business-and-professions-code/bpc-sect-17501/
67. 4 CCR § 1302 Former price — Justia Regulations — https://regulations.justia.com/states/california/title-4/division-3/article-10/section-1302
68. Cal. Civ. Code § 1770 (a)(13) — FindLaw — https://codes.findlaw.com/ca/civil-code/civ-sect-1770/
69. California Appellate Panel Upholds Validity of Pricing Statute — Manatt, 2019 — https://www.manatt.com/insights/newsletters/advertising-law/california-appellate-panel-upholds-validity-of-pri
