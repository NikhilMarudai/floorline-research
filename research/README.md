# Floorline research appendix

Floorline sets a price and a minimum on every item in a small furniture store, and checks every offer on the sales floor against that minimum. This folder is everything behind the claims on the site, the deck and the video. Built at VibeCon SF, October 2026.

Every number has a source. Each findings file has a Summary, numbered Findings with a source link and a confidence level, Tables, Gaps, and a Sources list, plus a JSON copy for filtering. Store details are anonymized: we're working with the owner-operator of a family-run store near Sacramento, California, and the store and its town are not named.

## Read it in story order

| # | Section | The short version | Headline numbers | Files |
|---|---|---|---|---|
| 1 | Why now | Pricing used to take a team. Now it takes AI and the data the store already has. | Small-business generative-AI use 23% (2023) → 58% (2025). US furniture stores 23,513 (2013) → 21,964 (2023). | [08](findings/08-inflection-point.md), [chart](charts/inflection.svg) |
| 2 | Customer | The mom-and-pop furniture store. The owner prices everything and isn't always there. | 20,098 small US furniture stores, 2,071 in California, ~$1.4M average revenue. About 1 in 5 US employer businesses is immigrant-owned. | [02](findings/02-industry-numbers.md), [11](findings/11-expansion-census.md), [owner interview](evidence/owner-interview.md) |
| 3 | Problem | Prices set by feel, retagged by hand, discounted below margin, and an owner on the phone all weekend. | 51% gross margin, so 10% off a $2,000 sofa costs the salesperson $12 and the store $200. Stock sits about 120 days. 48% of furniture buyers haggle; 89% of them win. | [02](findings/02-industry-numbers.md), [01](findings/01-pricing-layers.md), [05](findings/05-voc-reddit-forums.md), [06](findings/06-voc-reviews.md), [07](findings/07-voc-video.md), [invoice](evidence/invoice-redacted.jpg) |
| 4 | Solution | One place to set every price, and a minimum no one can sell below. | Minimum starts at a 25% margin and steps down at 3, 6 and 9 months. | [01](findings/01-pricing-layers.md), [story](story/story.md) |
| 5 | Product | Prices and minimums, the floor as a picture, sales in one place, a dashboard, questions in plain language, a deal check on the phone. ML pricing next. | Demo store: 300 items, $498,822 at cost, 400 deals (synthetic). | [data](data/SCHEMA.md), [story](story/story.md) |
| 6 | Evidence | A family store we're building with, a real invoice, 122 public voices, a citation on every number. | 122 public quotes: haggling 43, commission conflict 43, owner or manager approval 30. | [09](findings/09-owner-evidence.md), [05](findings/05-voc-reddit-forums.md), [06](findings/06-voc-reviews.md), [07](findings/07-voc-video.md) |
| 7 | Market | Furniture first, then any store that haggles, then any store that needs prices that move. | At today's prices: $61.5M (furniture), $580M (20 haggling trades), ~$2.7B (all small US retail). 5% of the first four trades ≈ $10.2M a year. | [14](findings/14-market-at-current-pricing.md), [13](findings/13-expansion-market.md), [11](findings/11-expansion-census.md), [12](findings/12-expansion-fit.md) |
| 8 | Competition | The pieces exist, scattered across registers, add-ons and enterprise software. Nobody combines them for a small store. | Registers $89–289/mo with a manager code; STORIS enterprise only; car dealers already pay $2,000+/mo. | [03](findings/03-existing-tools.md), [12](findings/12-expansion-fit.md) |
| 9 | Business model | $1,000 setup, then a monthly price per store. Full refund in 30 days. | Floor $200, Gallery $250, Forecast $450; digital tags (Sync) from $5,000 setup. | [10](findings/10-pricing-tiers.md), [15](findings/15-esl-costs.md) |
| 10 | Go-to-market | In through someone owners trust, then new and changing owners, then trade shows and buying groups. | The owner-operator's network: 10+ stores. Furniture First: 223 independents. HFA: 1,500+ members. | [04](findings/04-go-to-market.md) |
| 11 | Vision | Prices that learn from each store's sales, then jewelers, RV and boat dealers, secondhand stores, car lots. | Jewelers 19,396 small stores; RV/boat/powersports 11,323; secondhand 15,975; used cars 23,872. | [12](findings/12-expansion-fit.md), [13](findings/13-expansion-market.md) |
| 12 | Risks | Owners resisting new software, the floor experience, bigger players. Answer: store by store, through people owners trust. | | [story](story/story.md), Gaps sections in every findings file |

## What's in each folder

- `findings/` — 01 pricing inputs, 02 industry numbers, 03 existing tools, 04 go-to-market, 05–07 voice of customer (Reddit and forums, reviews, video), 08 why now, 09 owner evidence, 10 pricing pages, 11 expansion counts (Census), 12 expansion fit, 13 expansion market, 14 market at today's prices, 15 digital price tag costs.
- `evidence/` — the owner interview answers and a real invoice with every customer and store detail removed.
- `data/` — the synthetic demo store: inventory, sales history, staff and vendors, with the column dictionary. No real customers or staff.
- `charts/` — the "why now" chart (animated SVG, Census store counts).
- `story/` — the twelve sections as written for the site, deck and video.
- `deck/` — the deck.

## What's not here, on purpose
The original invoice, the raw interview recordings and transcripts, and anything with a real customer's or store's details. Quotes from public posts are verbatim and carry no usernames.
