# Owner evidence: a real invoice from the interviewed store

Generated: 2026-10-25 01:30 PDT · Agent: research-fork · Status: complete

Received from Nikhil by message on 2026-10-25 ~01:20 AM. One customer invoice from the interviewed owner's store, dated 6-20-26, invoice number 1291. The original photo is kept in `09-owner-evidence/invoice-1291-ORIGINAL-private.jpeg` and is **not for the website, the submission, the README or any public folder**: it carries a real customer's name, street address, phone, email, a finance account number and a signature, and the store's name, address and contact details. The redacted copy (re-done 06:20 AM) blacks out all of those, the store logo and the salesperson's initials; line items, fees, totals and policies stay visible. A redacted copy is `09-owner-evidence/invoice-1291-redacted.jpeg`. Everything below is read from the business side of the form; no customer detail is transcribed anywhere.

## Summary
- The store is a promotional-to-mid-tier furniture store near Sacramento, California, not an upscale gallery. Its name and address are kept private. [F-evidence-01]
- One ticket: a 5-piece dining set at $1,198 and a 5-piece bedroom set (bed frame, dresser, mirror, two nightstands) at $1,596, so $2,794 of merchandise. [F-evidence-02]
- Delivery was charged at $99 and assembly at $129; nothing was given free on this ticket. Subtotal $3,022, sales tax 8.75% $264.43, total $3,286.43. [F-evidence-03]
- Approximate ETA 2–4 weeks and a 90-day finance term; the policies box says special orders need a minimum 25% deposit, cancellations carry a 25% service charge, and delivery dates are estimates. [F-evidence-04, 05]
- The printed form has a Salesman box, so sales are attributed per person on paper already; it has no field for the price the item was tagged at, so a discount is invisible on the record. [F-evidence-06]

## Findings
### F-evidence-01 — The interviewed store is a discounter near Sacramento, California
- **Value:** a family-run furniture store (Mona runs it with her parents); store name, address and contact details kept private
- **Source:** Invoice 1291 header, store copy supplied by the owner
- **Confidence:** high
- **Use:** submission-research · pitch. Public wording: "a store near Sacramento, California." Never name the store or its town.

### F-evidence-02 — Average ticket on this invoice is $2,794 of merchandise
- **Value:** 5pc dining $1,198; 5pc bedroom $1,596 (bed frame, dresser, mirror, 2 nightstands)
- **Source:** Invoice 1291 line items
- **Confidence:** high, one ticket
- **Use:** submission-research · demo-data (the leakage estimate assumed a $2,000 average ticket, F-industry-29; one real ticket at $2,794 sits above it, so the assumption is not generous)

### F-evidence-03 — Delivery charged $99, assembly charged $129, tax 8.75%
- **Value:** Delivery fee $99; assembly fee $129; recycle fee blank; subtotal $3,022; sales tax 8.75% = $264.43; total payable $3,286.43
- **Source:** Invoice 1291 fee block
- **Confidence:** high
- **Use:** layer1-spec · demo-data (the research assumed a $99 standard delivery fee, F-industry-24; this confirms it exactly for this store. The app's concession table uses delivery $110 cost and assembly $40 cost to the store; the charged prices here are $99 and $129. Charged fee and cost to the store are different numbers; the waived-delivery leak is the fee, the cost is what the truck and crew cost.)

### F-evidence-04 — Lead time 2–4 weeks on this order; 90-day finance term
- **Value:** "Approx ETA (weeks): 2–4 wks"; finance term "90 days"; balance due noted as paid in full
- **Source:** Invoice 1291
- **Confidence:** high
- **Use:** layer1-spec (special-order lead times in the data run 10–16 weeks; this store's stock orders are 2–4 weeks; both exist)

### F-evidence-05 — Store policies that touch pricing
- **Value:** All sales final; floor models, clearance and discounted items not eligible for return; special orders may require a minimum 25% deposit and are not cancellable once placed; 25% service charge on approved cancellations or refunds; manufacturer warranty coverage limited to 30 days for pickup or delivery; delivery dates are estimates
- **Source:** Invoice 1291 "Company policies" block
- **Confidence:** high
- **Use:** layer1-spec (supports the special-order rule in the engine: deposit, no returns, so no reason to discount)

### F-evidence-06 — The form attributes the sale to a salesperson but records no tag price
- **Value:** Fields: Salesman, Quantity, Unit description, Unit price, Amount; no field for list or tag price, no field for discount
- **Source:** Invoice 1291 layout
- **Confidence:** high
- **Use:** pitch · product-insight (the paper record cannot show margin given away; the deal log is the first place that number exists)

## Tables

### What this changes in the research pack
| Item | Before | Now |
|---|---|---|
| Standard delivery fee | assumed $99 (F-industry-24) | confirmed $99 at this store |
| Average ticket | assumed $2,000 (F-industry-29) | one real ticket $2,794 |
| Store tier | described as a "gallery", mid-to-upper brands in the synthetic data | a discounter near Sacramento; promotional-to-mid price points ($1,198 dining set, $1,596 bedroom set) |
| Lead time | special orders 10–16 weeks | stock orders 2–4 weeks here; both should exist in the data |
| Sales tax for demo | none | 8.75% (local rate) if the deal log ever shows tax |

### How to use it in the flow
| Where | What | Condition |
|---|---|---|
| Submission research text | "One real invoice from the store we're working with: $2,794 of merchandise, delivery charged $99, assembly $129, 90-day finance." | Never name the store |
| Why page, the floor section | The $99 delivery fee as the number that gets waived | Text only; no image needed |
| Public site or README | The redacted image, captioned "an actual invoice from the interviewed store, customer details removed" | Only with the owner's explicit permission to show the document; otherwise text only |
| Demo data | Add a handful of $1,000–1,700 five-piece sets and 2–4 week lead times | Later, not before the build freeze |

## Gaps and unverified
- Permission: the owner agreed to be named. Nikhil, who is working directly with her, asked at 05:40 on 2026-10-25 for the redacted photo to go on the site, on condition that every identifying detail is crossed out (customer, store, address, contacts, salesperson). The redacted copy meets that; the original stays private.
- One invoice is one data point. It confirms the delivery fee and gives one ticket size; it does not establish averages.
- Salesman initials are now blacked out in the redacted copy.
- Handwritten entries read as: dining $1,198, bedroom $1,596, delivery 99, assembly 129, subtotal 3,022, tax 264.43, total 3,286.43. The arithmetic checks: 1,198 + 1,596 + 99 + 129 = 3,022; × 1.0875 = 3,286.43.

## Sources
1. Invoice 1291 from the store we're working with near Sacramento, 6-20-26, store copy photographed by the owner and sent to Nikhil 2026-10-25. Original: `09-owner-evidence/invoice-1291-ORIGINAL-private.jpeg` (private). Redacted: `09-owner-evidence/invoice-1291-redacted.jpeg`.
