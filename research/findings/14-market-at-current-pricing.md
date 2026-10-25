# Market size at today's pricing
Generated: 2026-10-25 ~06:40 PDT · Agent: research-fork · Status: complete

Recomputes the market for PriceLine's three tiers as built in Rounds T and T2: Floor $200, Gallery $250, Forecast $450 per store per month, billed from day one with a 30-day refund. Store counts are from `11-expansion-census.md` (Census County Business Patterns 2023, establishments with fewer than 20 employees). The expansion order is from `13-expansion-market.md`. The tier mix is an assumption, stated below. No published data gives the share of customers who pick each tier; the often-quoted "60–70% pick the middle" has no traceable source (`10-pricing-tiers.md`).

## Summary
- At a base mix of 50% Floor, 35% Gallery and 15% Forecast, the blended price is $255 a store a month, or $3,060 a year.
- US small furniture stores alone are a $61.5M annual ceiling at that price, up from the $48.2M the Market page shows at a flat $200.
- Furniture plus jewelers, RV, boat and powersports dealers, and secondhand stores (66,792 small stores) is a $204M ceiling. Adding used-car dealers (90,664 stores) makes $277M. All 20 trades (189,653 stores) make $580M.
- Ceilings assume every store subscribes. Realistic numbers: 5% of small furniture stores (about 1,005) is $3.1M a year; 5% of the phase 1–4 trades (about 3,340 stores) is $10.2M; 10% is $20.4M.
- The first 100 stores are about $306,000 a year at the base mix.

## Tier mix assumption

| Mix | Floor | Gallery | Forecast | Blended per month | Per year |
|---|---|---|---|---|---|
| Conservative | 70% | 25% | 5% | $225 | $2,700 |
| **Base** | **50%** | **35%** | **15%** | **$255** | **$3,060** |
| Stretch | 30% | 45% | 25% | $285 | $3,420 |

Gallery is marked "Most stores pick this" on the page, and the base case still puts half of stores on Floor. Forecast stays a minority because its model features are "coming". Additional stores at $135 a month are left out, since the counts are single establishments.

## Ceilings: every store subscribes

| Set | Small stores | All on Floor ($200) | **Base blend ($255)** | All on Forecast ($450) |
|---|---|---|---|---|
| US furniture stores, all sizes | 21,964 | $52.7M | **$67.2M** | $118.6M |
| US furniture stores, under 20 employees | 20,098 | $48.2M | **$61.5M** | $108.5M |
| California small furniture stores | 2,071 | $5.0M | **$6.3M** | $11.2M |
| Phases 1–4: furniture, jewelers, RV/boat/powersports, secondhand | 66,792 | $160.3M | **$204.4M** | $360.7M |
| Phases 1–5: plus used-car dealers | 90,664 | $217.6M | **$277.4M** | $489.6M |
| All 20 trades | 189,653 | $455.2M | **$580.3M** | $1,024.1M |

## What is reachable: penetration at the base blend

| Set | 1% | 5% | 10% |
|---|---|---|---|
| Small furniture stores (20,098) | 201 stores · $0.6M | 1,005 · $3.1M | 2,010 · $6.2M |
| Phases 1–4 (66,792) | 668 · $2.0M | 3,340 · $10.2M | 6,679 · $20.4M |
| Phases 1–5 (90,664) | 907 · $2.8M | 4,533 · $13.9M | 9,066 · $27.7M |

For scale: Clientbook, CarGurus and Lightspeed reached these buyers through the same buying groups and trade shows in the go-to-market plan (`04-go-to-market.md`). No penetration rate for this category is published, so 1%, 5% and 10% are scenarios, not forecasts.

## Changes this makes to the live Market page
The size tiles were computed at a flat $200 before the tiers existed ($52.7M, $48.2M, $5.0M, $240k). At today's prices and the base mix they become $67.2M, $61.5M, $6.3M and $306k. The page should state the mix in one line so the number is honest. The growth section (Round X) moves from flat-$200 figures to the base blend, plus the 5% scenario.

## Sources
Store counts: Census County Business Patterns 2023 via `11-expansion-census.md`. Expansion order and fit: `12-expansion-fit.md`, `13-expansion-market.md`. Tier prices: the live Market page after Rounds T and T2, as reported by the Emergent Coordinator, 2026-10-25. Tier-mix evidence (none published): `10-pricing-tiers.md`.

## Addendum, 05:45 AM: the outer ring
All US retail (NAICS 44-45, Census County Business Patterns 2023, all legal forms): 1,043,373 establishments, of which 877,627 have fewer than 20 employees (parsed from `11-work/dl/cbp23us.txt`, row `44----`, lfo `-`). At the base blend of $3,060 a year that is about $2.69B; all on Floor, about $2.11B. This ring includes grocery, gas stations and others where item-by-item pricing fits weakly, so it is a ceiling for "stores that need prices that move," not a plan.

Market circles for the site and deck: outer, all small retail, 877,627 stores, about $2.7B; middle, furniture plus the 19 related trades, 189,653, about $580M; inner, furniture, 20,098, about $61.5M; center, 5% of furniture, jewelers, RV and boat, and secondhand, about 3,340 stores, about $10.2M.
