# Sample data for the gallery pricing tool — schema and assumptions

Generated 2026-10-24 by `generate_inventory.py` (seed 20261024, Python standard library,
run with `python3 -I generate_inventory.py`). Everything here is synthetic: no real customers,
no real employees, no real store. Brand names are real so the numbers look right to a furniture
owner; collection and model names are invented but plausible. Re-running the script reproduces
the same files byte for byte.

## 1. The store being modelled (assumptions)

| Assumption | Value used |
|---|---|
| Format | Single-location independent gallery in California; mid-to-upper new branded furniture plus special-order pieces |
| Inventory on hand | about $500,000 at landed cost (the generator targets $500k ± $2.5k) |
| Staff | 3 sales (6% commission on sold price), 2 delivery, plus the owner. Owner sets a 10% discount authority for sales staff |
| Delivery | own truck; standard delivery charge $149; true cost to the store per trip $95–$180 |
| Categories | living room, bedroom, dining, home office, accents, mattresses (small share) |
| Vendors | 16 real brands independents carry (see `vendors.csv`) |
| Time window | inventory received over the last 36 months; sales history covers the last 6 months (2026-04-25 to 2026-10-24) |

Everything the owner said in the interviews that shaped this data: different cost multiples per
item (C-P039), staff discounting below the owner's comfortable minimum (C-P052, C-P055–056),
free delivery given away in negotiation (C-P044, C-P056), old stock sitting on the floor
(C-P049–050), discontinued / last-piece and 14-week lead-time items (A-S029–032), 6% sales
commission (B-S125–144), the $200-tag / $100-cost example (B-S106–124) and bundles with free
delivery (B-S255–259).

## 2. Files and columns

### inventory.csv — 300 rows, one per SKU

| Column | Type | Meaning |
|---|---|---|
| sku | text | Store SKU, `<category prefix>-<number>` (LR, BR, DN, HO, AC, MT) |
| name | text | Floor name: collection + piece type (+ width or rug size) |
| category | text | living room, bedroom, dining, home office, accents, mattresses |
| subcategory | text | sofa, sectional, recliner, accent chair, coffee table, end table, media console, bed, dresser, nightstand, chest, dining table, dining chair, sideboard, bar stool, desk, office chair, rug, lamp, mirror, art, occasional table, queen mattress, king mattress |
| vendor | text | Brand (see vendors.csv) |
| collection | text | Vendor collection / series (invented names) |
| material | text | Main cover or construction material |
| color | text | Color as it would read on the tag |
| color_family | text | neutral, warm, cool, bold (for grouping) |
| width_in, depth_in, height_in | integer | Dimensions in inches. Rugs: width × length, height 0 |
| unit_cost | money | What the store pays the vendor per unit |
| inbound_freight | money | Freight to get the unit to the store (3–13% of unit cost depending on category) |
| landed_cost | money | unit_cost + inbound_freight. This is the store's true cost basis |
| vendor_msrp | money | Vendor's suggested retail price |
| map_price | money or blank | Minimum advertised price for MAP brands; blank when the vendor has no MAP |
| tag_price | money | Price on the floor tag today |
| date_received | date | When the unit (first unit) arrived; YYYY-MM-DD |
| qty_on_hand | integer | Units in stock now, floor plus warehouse |
| units_sold_90d, units_sold_365d | integer | Units sold in the last 90 / 365 days (90d is always ≤ 365d). The 6-month figures reconcile to sales_history.csv; the older half of the year is simulated |
| floor_zone | text | Floor section A1–D4, or `warehouse` |
| reorder_lead_weeks | integer | Weeks to get another one from the vendor (2–16; special order 10–16) |
| discontinued | true/false | Vendor no longer makes it |
| last_unit | true/false | This is the last one; cannot be reordered |
| special_order | true/false | Floor sample of a made-to-order piece |
| trend_tag | text | Free-text merchandising note ("performance fabric", "curved", "warm wood", ... or blank) |
| image_url | text | Placeholder image, `https://placehold.co/600x400?text=<sku>` |

### staff.csv — 6 rows (5 staff + the owner)

| Column | Type | Meaning |
|---|---|---|
| staff_id | text | S01–S03 sales, D01–D02 delivery, OWN owner |
| name | text | Fictional name (deliberately unusual combinations; no real person intended) |
| role | text | sales, delivery, owner |
| commission_pct | number | 6.0 for sales, 0 otherwise |
| hire_date | date | YYYY-MM-DD |
| discount_authority_pct | integer | Largest discount off tag the person may give without calling the owner (10 for sales, 0 delivery, 100 owner) |

### sales_history.csv — 400 rows (deal lines), last 6 months

| Column | Type | Meaning |
|---|---|---|
| deal_id | text | D0001… in date order; one row per SKU sold |
| deal_group | text or blank | Bundle id (G001…G013) when several lines were sold together as one deal; blank for single-item deals |
| date | date | Close date |
| staff_id | text | Salesperson who closed it |
| sku | text | Item sold (joins to inventory.csv) |
| qty | integer | Units in the line |
| tag_price_at_sale | money | Tag price per unit when sold |
| sold_price | money | Price actually paid for the line (qty × negotiated unit price) |
| customer_offer | money | The customer's first offer for the line |
| delivery_charged | money | Delivery billed on this line ($149 standard, 0 if waived or carried out). In a bundle only the first line carries delivery |
| delivery_cost_to_store | money | What the trip cost the store (95–180; 0 when carried out or on later bundle lines) |
| concession_notes | text | free delivery, bundle discount, haul-away, none |
| owner_approved | true/false | Whether the owner approved the price before it was given |
| margin_dollars | money | sold_price + delivery_charged − landed_cost × qty − delivery_cost_to_store |
| margin_pct | number | margin_dollars ÷ sold_price × 100 |

### vendors.csv — 16 rows

| Column | Type | Meaning |
|---|---|---|
| vendor | text | Brand |
| tier | text | promotional, mid, better, best (price position) |
| has_map | true/false | Vendor enforces a minimum advertised price |
| typical_lead_weeks | integer | Normal reorder lead time |
| notes | text | One line on what the store buys from them |
| reference_url | text | Public page used to anchor the price band |

## 3. Price anchors (public pages checked 2026-10-24)

MSRP bands per vendor and category were set so generated tags fall inside what these pages show.
Sale prices on retailer pages move; the bands are ranges, not quotes.

| Brand | What was observed | Reference |
|---|---|---|
| Flexsteel | Charisma sofas target $999–$1,099; regular-line sofas $1,599–$1,899; leather / power reclining $2,700–$3,900 | https://homenewsnow.com/?p=17731 ; https://www.abt.com/rooms/flexsteel-linden-living-room |
| La-Z-Boy | Recliners $499–$4,000 depending on cover and power; most $999–$2,999 | https://furnitureacademy.com/la-z-boy-recliner-cost/ ; https://www.la-z-boy.com/b/recliners-gliding/_/N-1p87sqp |
| Stressless (Ekornes) | New recliners roughly $1,895–$4,495; Sunrise $2,495–$3,295 by leather grade | https://www.legacy.artplaceamerica.org/how-much-does-stressless-recliner-cost.html |
| Hooker Furniture | Dining tables about $1,266–$5,328 on sale | https://www.cymax.com/dining-tables--C626-7948-9566.htm |
| Magnussen Home | Queen panel beds $745–$1,595; 6-drawer dresser with mirror $1,148 sale / $2,325 list | https://www.cymax.com/Magnussen-Somerset--CL95506.htm ; https://colemanfurniture.com/lorelei-misty-cloud-queen-panel-bed.htm |
| Bassett | Ready-made sofas from $1,447 / $1,969 / $2,775; True Custom sofas $2,829–$4,909 | https://bassettfurniture.com/living/living-room-collections ; https://www.bassettfurniture.com/pdp/premier-custom-upholstery/classic-sofa/C100-72SF-3.html |
| Jonathan Louis | Sofas $899–$3,500, sectionals $2,800–$6,500 (estimate site plus retailer listings) | https://latestcost.com/jonathan-louis-sofa-price-typical-u-s-costs/ ; https://homemakers.com/shop/living-room/sofas-and-loveseats/sofas/jonathan-louis-bennett-indigo-sofa/13577S.html |
| Coaster | Sofas $589–$736; extendable dining set $1,380–$1,911 | https://colemanfurniture.com/ruth-coaster-furniture.html ; https://colemanfurniture.com/reseda-coaster-furniture.html |
| Universal Furniture | Queen canopy bed $6,990 sale / $8,738 list; 99" sofa $3,220 / $4,025 | https://colemanfurniture.com/cascade-universal.html ; https://colemanfurniture.com/leah-universal.html |
| Tempur-Pedic | Queen: Adapt $2,199; ProAdapt hybrid $3,399; ProBreeze $4,499 | https://www.pcrichard.com/sealy-tempur-pedic-savings/ |
| Sealy | Queen Posturepedic $1,499–$2,599 | https://www.pcrichard.com/queen-hybrid-mattreses/ |
| Loloi | 8x10-class rugs $729 (Magnolia Home) to $2,599 (hand-woven wool); shags from ~$420 | https://www.livingspaces.com/departments/rugs/area-rugs/8x10-wool-p135361-a50~376-a6~119 |
| Uttermost | Table lamps $270–$960 list; wall mirrors $150–$800 | https://isabelleslighting.com/mirah-olive-glass-table-lamp-30471/ ; https://www.rakuten.com/b/uttermost |
| Rowe, Craftmaster, Signature Design by Ashley | No clean public price list surfaced (Craftmaster dealers show "call for price"); bands set from the comparable tier above (Rowe/Craftmaster ≈ Bassett/Flexsteel; Ashley ≈ Coaster) | https://www.bigsandysuperstore.com/product/craftmaster-customizable-cm-modern-sofa-723450bd-1084717 |

MAP: La-Z-Boy, Flexsteel, Stressless, Signature Design by Ashley, Loloi, Tempur-Pedic and Sealy
are modelled as MAP vendors. That is common industry practice for these brands but no policy
document was retrieved during this run, so treat `has_map` as a modelling assumption.

## 4. How the generator builds the numbers

**Cost and price chain per SKU**

1. `vendor_msrp` is drawn from the subcategory band, scaled by the vendor's price factor
   (Coaster 0.55 … Stressless 1.9), and rounded to a tag-style price point.
2. `unit_cost` = MSRP ÷ a vendor "wholesale multiple" (2.3–2.6 for furniture, 2.7–3.0 for
   accessories, 1.9–2.1 for mattresses). `inbound_freight` = 3–13% of unit cost by category.
   `landed_cost` = unit_cost + inbound_freight.
3. `tag_price`:
   - Non-MAP vendors: landed × initial markup — **2.0–2.5× upholstery and case goods,
     2.5–3.0× accents, 1.9–2.2× mattresses** — capped at about MSRP.
   - MAP vendors: tag = max(MAP, landed × 1.8–2.1), so the markup is structurally lower.
   - Deliberate mistakes for the owner layer to catch: about 5% of non-MAP rows tagged 22–40%
     **over** the formula (ends above MSRP), about 6% tagged 16–28% **under** it (old tag never
     raised after a cost increase).
4. `map_price` for MAP vendors = 86–95% of MSRP.

**Aging skew.** `date_received`: ~62% in the last 12 months (triangular, peaking around 5
months), ~24% 12–24 months, ~14% 24–36 months. Items older than 18 months are much more likely
to be discontinued (22% vs 5%), sit at quantity 1, and live in zones C/D or the warehouse.

**Quantities.** Mostly 1–3; dining chairs 2–8, bar stools 2–6, lamps 2–8. Special-order and
aged rows are 1. After generation the script nudges quantities on recent, reorderable rows
until inventory at landed cost is within $2,500 of $500,000.

**Sales history.** 400 lines over 6 months. Items are drawn with weights so aged stock rarely
sells (24+ months: 0.12×; 12–24 months: 0.45×; accents 1.6×). Each salesperson has a discount
habit: S01 tight (mean 4.5%), S02 middle (8.5%), S03 loose (13.5%) with free delivery given on
12% / 28% / 47% of their deals respectively. MAP items are capped near 8% off. Aged items get
an extra 5–15% when they do move. Discounts above the 10% authority are only called in to
the owner about 62% of the time, the rest go through unapproved. A set of S03 deals is forced
to close at or below landed cost so there are visible "below floor" lines. 13 bundles
(2–4 lines each, shared `deal_group`) get an extra 2–6% off and usually free delivery; the truck
cost sits on the first line only. `units_sold_90d/365d` in inventory.csv are rebuilt from the
sales file (plus simulated older-half-year sales for items that were here long enough).

## 5. Summary statistics (from the generator run)

| Measure | Value |
|---|---|
| inventory.csv rows / units on hand | 300 / 704 |
| staff.csv rows | 6 (3 sales, 2 delivery, 1 owner) |
| sales_history.csv rows / bundle groups | 400 / 13 (38 bundle lines) |
| vendors.csv rows | 16 |
| Inventory at landed cost | **$498,822** |
| Inventory at tag | $1,072,638 |
| Average markup (tag ÷ landed): living room | 2.14× (112 rows, $194,045 at cost) |
| bedroom | 2.22× (60 rows, $95,556) |
| dining | 2.14× (48 rows, $83,662) |
| home office | 2.17× (11 rows, $40,092) |
| accents | 2.58× (59 rows, $35,929) |
| mattresses | 1.97× (10 rows, $49,538) |
| Rows received more than 12 months ago | 119 rows, $126,176 at cost |
| Rows received more than 24 months ago | 38 rows, $29,590 at cost |
| Discontinued / last unit / special order | 29 / 20 / 21 rows |
| MAP-priced rows | 75 |
| Deliberately over-priced / under-priced rows | 7 / 20 |
| 6-month revenue / gross margin after delivery | $592,141 / $274,044 (46.3%) |
| Deals with free delivery (truck rolled, nothing charged) | 94 lines (23.5%) |
| Deals below floor (negative margin after landed cost and delivery) | 14 lines, 11 of them by S03 |
| Deals discounted past the 10% authority | 157 lines, 57 with no owner approval |
| By salesperson — S01 | 122 lines, avg discount 5.6%, free delivery 4%, margin 51.5% |
| S02 | 141 lines, avg discount 10.0%, free delivery 29%, margin 45.4% |
| S03 | 137 lines, avg discount 17.2%, free delivery 35%, margin 41.3% |

Markups above are simple averages per row. MAP brands pull living-room and mattress averages
down, which is the intended effect.

## 6. Known simplifications

- One inbound freight figure per SKU; no handling, holding or floor-space cost is allocated.
- `vendor_msrp` for brands that publish only "starting at" prices is a modelled band.
- Sales history is six months only, so `units_sold_365d` includes simulated older sales.
- A special-order floor sample can show sales in the history (customer orders written against
  the sample); `qty_on_hand` stays at the sample count.
- Staff names are fictional. If any resembles a real person it is coincidence; rename freely.
