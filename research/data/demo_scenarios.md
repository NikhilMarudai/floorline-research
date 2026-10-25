# Demo scenarios — six rows that carry the 2-minute video

All rows come from `inventory.csv` / `sales_history.csv` (seed 20261024). Numbers below are
copied from the files; floor and negotiation framing is the product's job, not the data's.
Standard delivery is $149 charged, $95–$180 cost to the store.

| # | Story beat | SKU | Key numbers |
|---|---|---|---|
| 1 | The owner's own example: $200 tag, $100 cost | AC-0001 | tag $199, landed $100 (cost $94 + freight $6), MSRP $219, qty 4, sold 4 in 90 days |
| 2 | Aged piece worth clearing | LR-0001 | received 2024-08-03 (26 months), tag $2,699, landed $1,292, qty 1, zero sold in 12 months |
| 3 | Last unit, discontinued | DN-0001 | tag $1,999, landed $1,001, discontinued, last unit, 3 sold in 12 months |
| 4 | 14-week special order | LR-0002 | tag $4,999, landed $2,455, lead 14 weeks, 4 orders written in 90 days |
| 5 | MAP-protected brand | LR-0003 | tag $3,295 = MAP $3,295, MSRP $3,495, landed $1,835, qty 2 |
| 6 | 3-item bundle with delivery | deal group G008 | sofa + lamp + coffee table sold for $2,190 against $2,497 tag, free delivery ($107 cost), S03, margin $804 |

## 1. AC-0001 — Uttermost Revere Brass Table Lamp 28in (the $200 / $100 example)

- tag_price $199.00, landed_cost $100.00, vendor_msrp $219.00, no MAP, qty_on_hand 4, units_sold_90d 4, reorder 3 weeks, zone D2.
- This is the exact shape of the owner's spoken example (B-S106–124): $200 tag, $100 cost,
  customer offers $150. In the video: type the offer, show that $150 clears cost but leaves
  almost nothing after the salesperson's 6% ($9) and a share of the truck if it is delivered.
  Show the counter the tool suggests and the floor the owner set. It also sells steadily (4 in
  90 days), so there is no reason to go deep.

## 2. LR-0001 — Craftmaster Design Series 7718 Tuxedo Sofa 88in, mustard chenille (aged, clear it)

- date_received 2024-08-03 (about 26 months on the floor), tag_price $2,699.00, landed_cost
  $1,292.00, vendor_msrp $2,899.00, qty 1, units_sold_365d 0, zone B3, not discontinued.
- The "two years and it is still here" item (C-P049–050; B-S095–100). A bold color in a
  prime zone, never sold. In the video: the tool flags age and zero velocity, proposes a
  clearance price well below the normal floor (still above $1,292 landed) and shows what the
  floor space is worth to a fresh piece. Contrast with scenario 1 where the floor stays firm.

## 3. DN-0001 — Magnussen Home Westbourne 72in Sideboard (last unit, discontinued)

- tag_price $1,999.00, landed_cost $1,001.00, discontinued true, last_unit true, qty 1,
  received 2025-07-26, units_sold_365d 3 (it sold; this is the last of them), zone C1.
- Scarcity cuts both ways (A-S029–032): it cannot be reordered, so there is no "match the
  website" pressure, but it is also the end of a run and the next one will never come. In the
  video: show the tool holding the floor higher than for an ordinary aged item because the
  piece is proven (3 sold) and irreplaceable, while still allowing a modest concession to close.

## 4. LR-0002 — Rowe Townsend 3-Piece Modular Sectional, oatmeal performance fabric (14-week special order)

- tag_price $4,999.00, landed_cost $2,455.00, vendor_msrp $5,450.00, special_order true,
  reorder_lead_weeks 14, qty 1 (floor sample), units_sold_90d 4, zone A1, trend "modular".
- The fourteen-week example from the interview (A-S031–032). A hot sample (4 orders written in
  90 days) with a 14-week replacement. In the video: the tool refuses a deep discount on the
  floor sample because every sale here is a custom order at full price, and lead time is the
  customer's constraint, not the store's.

## 5. LR-0003 — Stressless Mayfair Signature Recliner with Ottoman, Medium, cognac leather (MAP brand)

- tag_price $3,295.00, map_price $3,295.00, vendor_msrp $3,495.00, landed_cost $1,835.00,
  qty 2, reorder 13 weeks, zone A3.
- Shows the layer the owner cannot override: the advertised price cannot go under MAP, so the
  negotiation moves to delivery, the ottoman, or an accessory instead of the number on the tag.
  In the video: a customer asks for 15% off; the tool explains why the tag stays and offers a
  concession menu that protects the dealer agreement.

## 6. Deal group G008 — the bundle (2026-10-12, salesperson S03)

| line | SKU | item | tag | sold | landed | delivery |
|---|---|---|---|---|---|---|
| 1 | LR-0046 | sofa | $1,549 | $1,425 | $796.85 | free (cost to store $107) |
| 2 | AC-0006 | lamp | $349 | $214 | $164.93 | — |
| 3 | LR-0017 | coffee table | $599 | $551 | $317.32 | — |

- Whole deal: $2,497 tag, $2,190 sold (12.3% off), free delivery, margin after landed cost and
  truck $804 (36.7%). The lamp went out at 39% off and the delivery was waived on top; the sofa
  line (the biggest one) was never approved by the owner.
- This is the couch-table-bookshelf question from the interview (B-S255–259): price the basket,
  not each line. In the video: show the tool evaluating the whole order with one truck trip,
  flagging that the lamp discount plus free delivery stacked past the 10% authority, and
  proposing the same closing price distributed so the salesperson stays inside the rules.

## Supporting cast (optional cutaways)

- S03 (Tobias Nakagawa-Reyes): 137 lines, average 17.2% off, free delivery on 35%, 11 of the
  14 below-floor deals in six months. The salesperson the owner is worried about (C-P055–056).
- S01 (Marisol Quintero-Vega): 5.6% average discount, 51.5% margin. The benchmark.
- Over-priced rows (tag above MSRP, e.g. BR-0014 Chapman Chest tag $1,899 vs MSRP $1,350) and
  under-priced rows show the owner layer fixing tags, not just guarding negotiations.
