# Pricing tiers and purchase page: layout references, per-location SaaS gating, strategy evidence, Stripe mechanics
Generated: 2026-10-25 · Agent: research-pricing-tiers · Status: partial (20-minute box; OpenAI and Toast pricing pages returned 403, so those rows rest on secondary sources dated Jun–Sep 2026)

Floorline planned tiers under test: $200 base (everything today) · ~$250 middle (gallery view) · $400–500 top (dynamic pricing from statistical models), per store per month. Competitor prices already on file (Lightspeed $89/$149/$289, Square Free/$89, Clientbook ~$295, Podium $399/2 locations, STORIS quote, CPQ $150–200/user) were not re-researched; they are reused below only where a layout or gating fact was needed.

## Summary
- Vertical per-location SaaS clusters at 1 : 1.7–2.7 : 3.2–10 between tiers (Lightspeed 89/149/289, Shopify 39/105/399, Prisync 99/199/399); consumer AI runs 1 : 5 : 10 (Claude Pro $20 → Max $100/$200; ChatGPT Plus $20 → Pro $100/$200). Floorline's 200/250/450 is 1 : 1.25 : 2.25, a flatter first step and a steeper second step than any peer [F-tiers-01, F-tiers-05, F-tiers-14].
- The one published rule of thumb with a named author (Rafi Mohammed, HBR 2013/2018, via secondary summaries): no more than four attributes differ per step, Good no more than ~25% below Better, Best no more than ~50% above Better. 200→250 passes (20% gap); 250→450 is +80% and fails unless the top tier carries more than one fence feature [F-tiers-09].
- Only one of the eight vendor pages fetched marks a tier: Square puts "Best value" on Plus (the middle paid tier). Claude, Shopify and Lightspeed mark nothing. A July 2026 scan of 301 pricing-page experiments found badge-style highlights in ~38%, usually on a mid or premium tier. The widely repeated "60–70% choose the middle tier" claim could not be traced to a primary ProfitWell source [F-tiers-02, F-tiers-10, F-tiers-11].
- Annual discounts observed: Claude 15%, ChatGPT Business 20%, Lightspeed "up to 18%", Shopify ~25%, Square none. The only survey figure found is SaaS Capital 2014 (52% offered a prepay discount, average 11.5%). Stripe's Atlas guide says make annual the default with a toggle to monthly [F-tiers-12, F-tiers-13].
- Trials: Square 30 days of Plus with no card; Prisync and RoomPriceGenie 14 days no card; Shopify 3 days then $1/month for 3 months; Lightspeed and Clientbook route to sales/demo. Stripe Checkout supports `subscription_data[trial_period_days]` up to 730 and card-optional trials with cancel/pause end behaviour [F-tiers-04, F-tiers-15, F-tiers-18].
- Stripe's no-code Pricing Table fits a 3-tier page (max 4 products, 3 prices each, highlight one product, trials, custom CTA on one product for "Talk to us") but cannot insert an account-creation step before Checkout; sign-in must happen before the table renders (pass a customer session) or after payment (from `checkout.session.completed`). Entitlements map `gallery_view` / `dynamic_pricing` features to products and fire `entitlements.active_entitlement_summary.updated` [F-tiers-17, F-tiers-19, F-tiers-21].

## Findings

### F-tiers-01 — Claude's consumer page runs five tiers at 1 : 5 : 10 with no "most popular" marker and comparison tables under the cards
- **Value:** Free $0; Pro $17/mo billed annually ($200 up front) or $20 monthly; Max "From $100" with "Choose 5x or 20x more usage than Pro" ($100 / $200 per month, monthly only); Team Standard seat $20 annual / $25 monthly, Premium seat $100 / $125; Enterprise $20/seat/month annual, 20-seat minimum, plus usage at API rates. Individual and Team/Enterprise are separate tabs. No toggle: both prices sit on the card. CTAs: "Try Claude" (all individual tiers), "Get Team plan", "Get Enterprise plan" + "Chat with buying specialist". Limits are relative multipliers ("More usage", "5x or 20x more usage than Pro", "5x more usage than standard seats") not message counts. Feature comparison tables follow the cards for both tabs. (2026-10-25)
- **Source:** [Pricing](https://claude.com/pricing) — Anthropic, fetched 2026-10-25
- **Confidence:** high (fetched official page); "Try Claude" leading to sign-in before plan selection is observed behaviour, not stated on the page
- **Use:** layer1-spec

### F-tiers-02 — ChatGPT runs Free / Go / Plus / Pro ×2 / Business / Enterprise; Plus is the de facto "most popular" and limits are message counts per window
- **Value:** Free $0; Go ~$8/mo; Plus $20/mo; Pro $100 or $200/mo (5x / 20x Plus usage); Business $20/user/mo annual or $25 monthly, 2-user minimum; Enterprise custom. Limits phrased as counts ("Up to 10 messages every 5 hours", "Up to 160 messages every 3 hours") and as multiples of Plus. Secondary sources call Plus "the most popular sweet spot"; one reports Go badged "Most Popular". Business is the only tier with an annual discount (20%). (Sep 2026)
- **Source:** [ChatGPT Pricing 2026: Free vs Go vs Plus vs Pro](https://www.cometapi.com/chatgpt-pricing-2026-free-vs-go-vs-plus-vs-pro/) — CometAPI, updated 2026-09-03; [ChatGPT pricing 2026](https://eesel.ai/blog/chatgpt-pricing) — eesel, checked against official sources 2026-09-09. Official page [openai.com/chatgpt/pricing](https://openai.com/chatgpt/pricing/) returned 403.
- **Confidence:** medium (two secondary sources agree on prices; the badge, toggle and comparison-table layout are not verified)
- **Use:** layer1-spec

### F-tiers-03 — Lightspeed Retail: three tiers at 1 : 1.7 : 3.2, "Contact sales" on every card, annual saves "up to 18%"
- **Value:** Basic $89, Core $149, Plus $289 per month (annual billing); monthly billing $109 / $179 / $339 per NerdWallet. Each tier includes one register; "Extra locations" and "Additional registers" are listed without prices. Gates: Basic→Core adds full eCommerce, accounting integrations, advanced reporting, loyalty, mobile app; Core→Plus adds omnichannel loyalty/rewards and advanced customization. No tier highlighted. CTA per card "Contact sales"; page header "Start a free trial"; trial length not stated. (2026)
- **Source:** [Retail POS pricing](https://www.lightspeedhq.com/pos/retail/pricing/) — Lightspeed, fetched 2026-10-25; [Lightspeed Retail POS Review 2026](https://www.nerdwallet.com/reviews/small-business/lightspeed-retail-pos) — NerdWallet, 2026
- **Confidence:** high for prices and CTA (official page); medium for monthly rates and gate detail (NerdWallet)
- **Use:** layer1-spec | pitch

### F-tiers-04 — Square for Retail: Free / Plus $89 per location / Premium custom, "Best value" badge on Plus, 30-day no-card trial
- **Value:** Free $0; Plus $89 per month per location; Premium custom (eligibility: >$250K processed per year); Square Pro custom. Gates: Free→Plus adds inventory management and stock intake, vendor/purchase orders, COGS reporting; Plus→Premium adds cross-location returns and fulfilment, transfer orders, 24/7 phone support. Plus is labelled "Best value". CTAs: "Get started" (Free), "Try free for [30] days" (Plus/Premium), "Talk to our team" (Pro). Anyone who signs up gets a 30-day trial of Plus with no payment information. No annual discount found. (2026)
- **Source:** [Square for Retail pricing](https://squareup.com/us/en/point-of-sale/retail/pricing) — Square, fetched 2026-10-25; [Square for Retail features](https://square.com/us/en/point-of-sale/retail/features) — Square; [Square for Retail Plans](https://squareup.com/help/au/article/6921) — Square help
- **Confidence:** high (official pages; prices from features page because the pricing page rendered without numbers)
- **Use:** layer1-spec

### F-tiers-05 — Shopify: Basic / Grow / Advanced at 1 : 2.7 : 10.2, ~25% annual discount, staff-account count is the main fence
- **Value:** Basic $39 monthly / $29 yearly; Grow $105 / $79; Advanced $399 / $299; Plus from $2,300. Gates: Basic→Grow adds up to 5 staff accounts (Basic 0), lower card rate (2.7% vs 2.9% + 30¢), bigger shipping discounts; Grow→Advanced adds 15 staff accounts, live third-party shipping rates, regional tailoring, 2.5% rate; Plus adds unlimited staff, custom checkout, 24/7 priority phone support. POS Pro add-on $89/mo per location. Trial: 3 days free then $1/month for 3 months, no card required. CTA "Start for free" on all three; "Try for $399" on Plus. No tier highlighted. (2026)
- **Source:** [Shopify pricing](https://www.shopify.com/pricing) — Shopify, fetched 2026-10-25
- **Confidence:** high
- **Use:** layer1-spec

### F-tiers-06 — Toast and Clover: restaurant/retail POS with a $0 entry tier, a ~$69 paid tier, and quote-based top; AI assistant bundled, not sold as a tier
- **Value:** Toast: Starter Kit $0/mo (higher processing), Point of Sale $69/mo (first terminal included), Build Your Own custom; add-ons Online Ordering $75/mo, Marketing $75/mo, Loyalty $25/mo, Mobile Order & Pay $25/mo per location; Toast IQ AI assistant reported as included at no extra cost. Clover (per device): Payments Plus $14.95, Essentials $29.95–54.95, Register $69.95, Counter Service $79.95, Table Service $89.95; additional devices ~$14.95/device. (Jun–Sep 2026)
- **Source:** [Restaurant POS pricing in 2026](https://www.katalystos.com/blog/restaurant-pos-pricing-in-2026-real-costs-from-every-major-vendor) — Katalyst (vendor blog), 2026-06-02, corrected 2026-09-08; [Clover POS Pricing Breakdown](https://www.upmenu.com/blog/clover-pos-pricing) — UpMenu, 2026. Official [pos.toasttab.com/pricing](https://pos.toasttab.com/pricing) returned 403.
- **Confidence:** low-medium (secondary, sources disagree on Clover tier names; Toast $0/$69 consistent across three sources)
- **Use:** layer1-spec

### F-tiers-07 — Clientbook publishes no tiers or prices; CTA is "Schedule a Demo" and a "personalized quote for your store"
- **Value:** The pricing-plans page lists no tier names, prices, or inclusions; copy reads "Schedule a free demo and we'll help you decide which plan is best for you and your business." No trial. PricingSaaS tracks it as "Pricing not disclosed" Q3 2025–Q1 2026. The ~$295/store figure on file is therefore a quote, not a list price. (2026)
- **Source:** [Clientbook pricing plans](https://www.clientbook.com/pricing-plans) — Clientbook, fetched 2026-10-25; [Clientbook Pricing Plans & History](https://pricingsaas.com/companies/clientbook) — PricingSaaS, 2026
- **Confidence:** high
- **Use:** pitch

### F-tiers-08 — No furniture-specific vendor publishes tiers; Furniture Wizard, STORIS, Frog, RetailVista, Myriad are all quote-only
- **Value:** Furniture Wizard: "Available upon request" (Software Advice). STORIS: quote-only (already on file). Frog, RetailVista, Myriad: no price found. Nearest published general-retail figure: Celerant basic plan $125/month (one POS, up to five back offices). Floorline would be the only furniture-vertical tool with a public three-tier page. (2026)
- **Source:** [Furniture Wizard profile](https://www.softwareadvice.com/retail/furniture-wizard-profile) — Software Advice, 2026; [5 Best Furniture Store Software](https://fitsmallbusiness.com/best-furniture-store-software/) — Fit Small Business, 2026
- **Confidence:** medium (absence of evidence after one search pass; Celerant figure is secondary)
- **Use:** pitch | submission-research

### F-tiers-09 — Mohammed (HBR): at most four attributes differ per step, Good no more than ~25% below Better, Best no more than ~50% above Better, define fence features first
- **Value:** Guidance as summarized from Rafi Mohammed's HBR work: no more than four attributes should differ between Good and Better or Better and Best; lower-tier features carry upward; Good should not be priced more than 25% below Better; Best not more than ~50% above Better; "fence" attributes stop existing customers trading down and should be defined first; expected revenue split Good 10–20%, Better 25–50%, Best 30–60%; a three-option set often leads buyers to the middle. Wikipedia adds the Williams-Sonoma anchor case (a $429 bread machine nearly doubled sales of the $279 model) and a jewellery-trade rule: Better ~10% above average ticket, Good ~25% lower, Best no more than 50% higher. (2013/2018)
- **Source:** [The Good-Better-Best Approach to Pricing](https://hbr.org/2018/09/the-good-better-best-approach-to-pricing) — HBR, Sep–Oct 2018 (paywalled; opening only fetched); [summary](https://theproductperson.substack.com/p/the-good-better-best-approach-to) — The Product Person (Substack); [Good–better–best](https://en.wikipedia.org/wiki/Good%E2%80%93better%E2%80%93best) — Wikipedia, incl. Mohammed 2013 "Why Good-Better-Best Prices Are So Effective"
- **Confidence:** medium (rules come via secondary summaries of a paywalled article; the "50%" wording is ambiguous in the summary)
- **Use:** layer1-spec | pitch

### F-tiers-10 — "Most popular" badges appear in roughly 38% of detected pricing-page experiments and sit on a mid or premium tier; lift is not measured
- **Value:** Scan of 301 pricing pages (July 2026): badge-style highlights in ~38% of detected experiments, usually on the mid or premium column; the authors state these are detected UI diffs, not measured conversion lift. Among the pages fetched here, only Square badges a tier ("Best value" on Plus); Claude, Shopify, Lightspeed do not. (2026)
- **Source:** [What % of pricing pages highlight a 'Most popular' plan](https://www.lazyweb.com/research/most-popular-badge-prevalence-pricing-pages) — Lazyweb Labs, July 2026, n=301
- **Confidence:** medium (small independent study, prevalence not causation)
- **Use:** layer1-spec

### F-tiers-11 — The "60–70% pick the middle tier" statistic is unsourced; the strongest middle-option evidence is the decoy effect, not SaaS data
- **Value:** Monetizely attributes "60–70% of customers pick the middle tier" and "+60% selection when the preferred plan is centred" to ProfitWell, and a "+25% from a Most Popular label" to CXL; none links to a primary study, and no Paddle/ProfitWell/OpenView report with these numbers was found. Price Intelligently's 512-company analysis (also secondhand) found four-tier companies often show higher LTV than three-tier. Treat the middle-tier share as unknown. (2026)
- **Source:** [Does the three-tier pricing model still work in SaaS](https://www.getmonetizely.com/articles/good-better-best-does-the-three-tier-pricing-model-still-work-in-saas) — Monetizely (vendor blog), 2026
- **Confidence:** low (secondary, unverifiable)
- **Use:** layer1-spec

### F-tiers-12 — Annual prepay discounts observed on fetched pages: 15% (Claude Pro), 20% (ChatGPT Business, Claude Team), up to 18% (Lightspeed), ~25% (Shopify), 0% (Square)
- **Value:** Claude Pro $17 vs $20 = 15%; Claude Team $20 vs $25 = 20%; ChatGPT Business $20 vs $25 = 20%; Lightspeed "save up to 18%" ($89 vs $109 = 18%); Shopify $29 vs $39 = 26%, $79 vs $105 = 25%, $299 vs $399 = 25%; Square lists no annual option. (2026)
- **Source:** pages cited in F-tiers-01 to F-tiers-05
- **Confidence:** high (computed from fetched prices)
- **Use:** layer1-spec

### F-tiers-13 — Survey baseline for prepay discounts: 52% of SaaS companies offered one, average 11.5% (SaaS Capital 2014); 15–20% is the common rule of thumb; Stripe Atlas says make annual the default
- **Value:** SaaS Capital 2014 survey of 200+ SaaS companies: 52% offered up-front payment discounts, average 11.5%. Monetizely calls 15–20% "the most prevalent discount model". Stripe Atlas guide (Patrick McKenzie): make the yearly plan the core offering with a toggle to monthly; one month free is a common format; keep the credit card requirement on trials ("Removing the card usually increases signups but lowers activation and conversion"); about three plans plus a "Call us" enterprise tier; use "Call us"/"Speak with us" not "Choose plan" on that tier. (2014/2026)
- **Source:** [What's the true cost of offering pre-pay discounts](https://www.saas-capital.com/research/whats-the-true-cost-of-offering-pre-pay-discounts-to-saas-customers/) — SaaS Capital, 2014 survey; [SaaS pricing guide](https://stripe.com/guides/atlas/saas-pricing) — Stripe Atlas; [Annual prepayment discount FAQ](https://www.getmonetizely.com/faqs/what-kind-of-discount-should-we-offer-for-annual-prepayment-versus-monthly-is-the-typical-approach-to-give-2-months-free-about-16-17-off-or-do-some-companies-do-a-different-discount-for-yearly-plans) — Monetizely
- **Confidence:** medium (survey is old; Atlas guide is opinion from a credible operator)
- **Use:** layer1-spec

### F-tiers-14 — Prisync gates its "Dynamic Pricing Engine" to the middle and top tiers at 1 : 2 : 4
- **Value:** URL-based model: Professional $99 (100 products), Premium $199 (1,000), Platinum $399 (5,000); channel-based $199/$399/$599; hybrid $299/$599/$799. Dynamic Pricing Engine included in Premium and Platinum, not Professional. 14-day free trial, no card, no contract. No annual discount shown. (2026)
- **Source:** [Prisync pricing](https://prisync.com/pricing/) — Prisync, fetched 2026-10-25
- **Confidence:** high
- **Use:** layer1-spec | pitch

### F-tiers-15 — RoomPriceGenie sells hotel dynamic pricing in three quote-based tiers that step up on forecast horizon, refresh frequency, history depth and human review
- **Value:** Core / Premium / Professional, priced per property by room count, "Contact Sales" on each, 14-day trial no card, annual commitment with monthly or upfront payment. Gates: future price recommendations 12 → 18 → 18 months; automated price uploads 4x → 24x → 24x daily; revenue dashboard 3-month → 2-year; onboarding standard → VIP; strategy reviews annual → quarterly; dedicated revenue manager only on Professional. HotelTechReport lists a $500/month base; Duetto is quote-only (estimates $200–500/property/month from a competitor blog, $1,000/month start per HotelTechReport); IDeaS price not found; Omnia Retail and Competera quote-only; PriceLabs ~$19.99/listing with a 30-day trial. (2026)
- **Source:** [RoomPriceGenie pricing](https://roompricegenie.com/pricing/) — RoomPriceGenie, fetched 2026-10-25; [Duetto pricing](https://www.g2.com/products/duetto/pricing) — G2; [Duetto Pricing 2026](https://www.roommaster.com/blog/duetto-pricing) — RoomMaster (competitor blog); [PriceLabs](https://hello.pricelabs.co/pricing/) — PriceLabs
- **Confidence:** high for RoomPriceGenie gates; low for Duetto estimates
- **Use:** layer1-spec | pitch

### F-tiers-16 — Stripe's packaging guidance: two to four tiers, each plan describable as one customer type in one sentence; a value metric must be understandable, hard to game and aligned with how buyers budget
- **Value:** "Two to four tiers are ideal: if you have more than four, buyers could struggle to compare options." Four value-metric properties: flexible with customer value, understandable without explanation, hard to game, aligned with how customers budget (maps to a line item buyers already track). Packaging levers: feature gating, usage limits rising across tiers, add-ons kept outside tiers. Upgrade triggers: team growth, collaboration, governance, volume. (2026)
- **Source:** [SaaS pricing and packaging strategy](https://stripe.com/resources/more/saas-pricing-and-packaging-strategy) — Stripe, 2026
- **Confidence:** high (fetched)
- **Use:** layer1-spec

### F-tiers-17 — Stripe Pricing Table: no-code 3-tier page with highlight, trials and one custom CTA; max 4 products × 3 prices, no account step before Checkout
- **Value:** Dashboard-built `<stripe-pricing-table>` web component. Supports flat-rate, per-seat, tiered and free trials; highlight one product; customize language, colours, font, button; up to four products per interval, three prices per product, three intervals total; one product may carry a custom CTA to any URL (for "Talk to us"); `customer-email`, `client-reference-id`, and `customer-session-client-secret` (30-minute window) to attach an authenticated customer; trial without card via "Only collect payment method information if required". Limitations: no usage-based pricing, "doesn't currently support adding an intermediate step (for example, asking the customer to create an account on your website before checking out)", 50 reads/second, needs a real domain to render. (2026)
- **Source:** [Embeddable pricing table for subscriptions](https://docs.stripe.com/payments/checkout/pricing-table) — Stripe Docs, fetched 2026-10-25
- **Confidence:** high
- **Use:** layer1-spec

### F-tiers-18 — Stripe Checkout trials: `subscription_data[trial_period_days]` up to 730, card-optional with cancel/pause end behaviour, reminder email required for compliance
- **Value:** `mode=subscription` + `subscription_data[trial_period_days]=30` (or `trial_end` timestamp); max 730 days, docs note "most businesses use shorter trials, such as 30 days". `payment_method_collection=if_required` skips the card; `subscription_data[trial_settings][end_behavior][missing_payment_method]=cancel|pause`. Dashboard can auto-send a trial-ending reminder with a link to add a card; `customer.subscription.trial_will_end` webhook for custom flows; card-network trial compliance rules apply. (2026)
- **Source:** [Configure free trials for Checkout](https://docs.stripe.com/payments/checkout/free-trials?ui=full-page) — Stripe Docs, fetched 2026-10-25
- **Confidence:** high
- **Use:** layer1-spec

### F-tiers-19 — Stripe Customer Portal: "Switch plan" is described as best for good-better-best; proration and end-of-period downgrades are toggles; max 10 products; trialing subscriptions need `continue_trial`
- **Value:** Dashboard options: Switch plan ("best when you have a good-better-best pricing model", default off), Update quantities, Prorate subscription updates (immediate or end of period), Manage downgrades (schedule at period end, same product only), promotion codes, cancellation with reasons and retention coupons. Limits: at most 10 products offered for switching; subscriptions with trials, multiple products or usage-based items can be cancelled but not updated; customer edits to a `trialing` subscription end the trial and invoice unless `features.subscription_update.trial_update_behavior=continue_trial`; portal cannot run in an iframe; sessions expire after 5 minutes unused. (2026)
- **Source:** [Configure the customer portal](https://docs.stripe.com/customer-management/configure-portal) and [Customer portal overview](https://docs.stripe.com/customer-management) — Stripe Docs, fetched 2026-10-25
- **Confidence:** high
- **Use:** layer1-spec

### F-tiers-20 — Stripe Link: email + one-time passcode identifies a returning buyer and autofills card and address inside Checkout; not an account system
- **Value:** Link detects enrolment by email, phone or cookie, sends a one-time passcode, then autofills saved card/bank details and addresses. Works in Checkout, Payment Links, Elements, Invoicing; enabled in payment-method settings. Not available in India. It authenticates payment details, not the Floorline account; app sign-in still has to be handled separately. (2026)
- **Source:** [Increase conversion and reduce costs with Link](https://docs.stripe.com/payments/link) — Stripe Docs, fetched 2026-10-25
- **Confidence:** high
- **Use:** layer1-spec

### F-tiers-21 — Stripe Entitlements: Feature objects with `lookup_key` attached to products; one webhook carries the customer's full active-feature list (max 10 inline)
- **Value:** Create features (`POST /v1/entitlements/features`, unique `lookup_key` such as `gallery_view`, `dynamic_pricing`), attach to products (`POST /v1/products/{id}/features`), then listen to `entitlements.active_entitlement_summary.updated` (fires on create, upgrade, downgrade, cancel, failed-payment cancel; payload lists up to 10 entitlements, more via `entitlements.url`) or call `GET /v1/entitlements/active_entitlements?customer=`. Feature changes to existing subscriptions take effect at the next billing period. Stripe recommends persisting entitlements internally. Subscription `metadata` remains the fallback for anything not modelled as a feature. (2026)
- **Source:** [Entitlements (API)](https://docs.stripe.com/billing/entitlements?dashboard-or-api=api) — Stripe Docs, fetched 2026-10-25
- **Confidence:** high
- **Use:** layer1-spec

## Tables

### (a) Layout comparison

| Vendor | Tiers and prices (per month) | Price ratio | Most-popular marker | Monthly/annual toggle | Comparison table below cards | CTA wording | Sign-in before pay? | URL |
|---|---|---|---|---|---|---|---|---|
| Anthropic Claude | Free $0 · Pro $17 annual / $20 monthly · Max $100 (5x) / $200 (20x) · Team $20–25 Std, $100–125 Premium per seat · Enterprise $20/seat annual, 20-seat min | Pro : Max = 1 : 5 : 10 | None in page text | No toggle; both prices on card; Individual vs Team & Enterprise tabs | Yes (one per tab: features, security, payment, models) | "Try Claude" / "Get Team plan" / "Get Enterprise plan" / "Chat with buying specialist" | Yes: "Try Claude" opens claude.ai sign-in, plan chosen inside the app (observed) | claude.com/pricing |
| OpenAI ChatGPT (secondary) | Free $0 · Go ~$8 · Plus $20 · Pro $100 / $200 · Business $20 annual / $25 monthly per user, 2-seat min · Enterprise custom | Plus : Pro = 1 : 5 : 10 | Plus per secondary ("sweet spot"); not verified on page | Personal/Business tabs; annual only on Business (not verified) | Not verified (page 403) | Not verified ("Get Plus"/"Get Pro" pattern per secondary) | Yes: chatgpt.com account before upgrade (observed) | openai.com/chatgpt/pricing (403); cometapi.com, eesel.ai summaries |
| Lightspeed Retail | Basic $89 · Core $149 · Plus $289 (annual); $109 / $179 / $339 monthly | 1 : 1.7 : 3.2 | None | "Save up to 18%" annual; prices shown at annual rate | Feature list per card; no separate matrix fetched | "Contact sales" per card; "Start a free trial" header; "Schedule a call" multi-location | Sales-led; trial via form | lightspeedhq.com/pos/retail/pricing |
| Shopify | Basic $39/$29 · Grow $105/$79 · Advanced $399/$299 · Plus from $2,300 | 1 : 2.7 : 10.2 | None | Yes (monthly / yearly) | Yes (full feature matrix) | "Start for free" ×3; "Try for $399" (Plus) | Account created in trial sign-up before any charge | shopify.com/pricing |
| Square for Retail | Free $0 · Plus $89 per location · Premium custom (>$250K/yr) · Square Pro custom | 0 : 1 : quote | "Best value" on Plus | No annual option | Feature bullets per tier | "Get started" / "Try free for 30 days" / "Talk to our team" | Square account sign-up first; 30-day Plus trial, no card | squareup.com/us/en/point-of-sale/retail/pricing |
| Toast (secondary) | Starter Kit $0 · Point of Sale $69 · Build Your Own custom | 0 : 1 : quote | Not verified | Not verified | Not verified | Not verified | Sales-led | pos.toasttab.com/pricing (403) |
| Clientbook | No published tiers | n/a | n/a | n/a | n/a | "Schedule a Demo" / "Book a Demo" | Demo, then quote | clientbook.com/pricing-plans |
| Prisync | Professional $99 · Premium $199 · Platinum $399 (URL-based) | 1 : 2 : 4 | Not noted | Not shown | Feature list per tier | Free trial (14 days, no card) | Trial sign-up first | prisync.com/pricing |
| RoomPriceGenie | Core · Premium · Professional, quote per property | quote | None | Annual commitment, monthly or upfront payment | Yes (feature matrix) | "Contact Sales"; 14-day trial, no card | Trial sign-up first | roompricegenie.com/pricing |

### (b) Gating table

| Vendor | What separates tier 1→2 | What separates 2→3 | Add-ons | Trial |
|---|---|---|---|---|
| Claude | Pro: "More usage" (≥5x Free), more models, projects, connectors | Max: 5x or 20x Pro usage, higher output limits, early access | Team Premium seat (5x Std); Enterprise usage at API rates | Free tier is the trial |
| ChatGPT | Plus: higher message caps (e.g. 160/3h vs 10/5h), better models | Pro: 5x / 20x Plus usage, unlimited on flagship models | Business seats; Enterprise custom | Free tier is the trial |
| Lightspeed Retail | Core: full eCommerce, accounting integrations, advanced reporting, loyalty, mobile app | Plus: omnichannel loyalty/rewards, advanced customization, scalability | Extra locations, additional registers (unpriced); Payments 1.5–2.6% | Not stated on page; sales-led |
| Shopify | Grow: 5 staff accounts (vs 0), 2.7% card rate, 87% shipping discounts | Advanced: 15 staff accounts, live carrier rates, regional tailoring, 2.5% rate | POS Pro $89/mo per location; Plus unlimited staff, custom checkout, 24/7 priority phone | 3 days free, then $1/mo × 3 months, no card |
| Square for Retail | Plus: inventory management and stock intake, vendor/purchase orders, COGS reporting | Premium: cross-location returns and fulfilment, transfer orders, 24/7 phone support | Per-location pricing; Square Pro: hardware discounts, onboarding, account manager | 30 days of Plus, no card |
| Toast | Point of Sale: lower processing (2.49% vs ~3.09%), full POS | Build Your Own: multi-location, volume pricing | Online Ordering $75, Marketing $75, Loyalty $25, Mobile Order & Pay $25/location; Toast IQ AI included | None found |
| Prisync | Premium: 1,000 products, Dynamic Pricing Engine | Platinum: 5,000 products, extra features | Channel-based and hybrid models at higher price points | 14 days, no card |
| RoomPriceGenie | Premium: 18-month horizon (vs 12), 24x daily uploads (vs 4x), 2-year dashboard (vs 3-month), advanced min-stay automation | Professional: VIP onboarding, quarterly strategy reviews, dedicated revenue manager | Priced by room count | 14 days, no card |

### (c) What this implies for Floorline

| # | Recommendation | Evidence | Source IDs |
|---|---|---|---|
| 1 | Keep three visible tiers plus a hidden fourth "Multi-store: talk to us" link; do not show a free tier | Stripe: 2–4 tiers ideal; Atlas: ~3 plans + "Call us" enterprise, "free is not a compelling value proposition" to funded buyers; furniture peers (STORIS, Furniture Wizard, Clientbook) are all quote-only, so a public 3-tier page is itself a differentiator | F-tiers-16, F-tiers-13, F-tiers-07, F-tiers-08 |
| 2 | Re-examine the 200 / 250 / 450 ladder: either widen the first step or narrow the second. Options that fit Mohammed's bounds: $200 / $300 / $450 (1 : 1.5 : 2.25) or $200 / $250 / $375 (1 : 1.25 : 1.9). If $450–500 stays, the top tier needs 3–4 visible fences, not just "dynamic pricing" | Mohammed: Good ≤25% below Better (200→250 = 20%, passes), Best ≤50% above Better (250→450 = +80%, fails); peers run 1 : 1.7 : 3.2 (Lightspeed), 1 : 2 : 4 (Prisync), 1 : 2.7 : 10 (Shopify) | F-tiers-09, F-tiers-03, F-tiers-05, F-tiers-14 |
| 3 | Badge the middle tier ("Most popular" or Square's "Best value"); highlight it in the Stripe Pricing Table; do not claim a "60–70% choose middle" stat in the pitch | Square badges Plus; ~38% of pricing-page experiments carry a badge, usually mid/premium; three options steer to the middle (Mohammed, Williams-Sonoma anchor); the 60–70% figure is untraceable | F-tiers-04, F-tiers-10, F-tiers-11, F-tiers-09, F-tiers-17 |
| 4 | Value metric: flat per store per month, unlimited salesperson phones, no per-seat line; price a second store as an add-on (e.g. 50% of base) rather than a separate tier | Square, Lightspeed, Shopify POS all price per location; Shopify's seat-count fence is the pattern to avoid because salesperson turnover is high (03/04 files); Stripe's four properties: aligned with how buyers budget (owners already pay POS per location), hard to game, understandable | F-tiers-16, F-tiers-04, F-tiers-03, F-tiers-05 |
| 5 | Offer monthly and annual with a toggle; annual at two months free (~17%); show the annual-equivalent price on the card like Claude ($17 "billed annually") | Observed 15–25% across Claude, ChatGPT Business, Lightspeed, Shopify; SaaS Capital average 11.5%; Atlas: make annual the default with monthly toggle; Pricing Table supports up to three intervals | F-tiers-12, F-tiers-13, F-tiers-17 |
| 6 | Trial: 30 days of the middle tier with card on file (Checkout `trial_period_days=30`, reminder email on), falling back to the base tier if they do nothing; enterprise/multi-store gets a pilot call instead | Square's 30-day Plus trial is the direct per-location analog; dynamic-pricing vendors use 14 days; Atlas: keep the card requirement; Stripe docs: 30 days typical, `missing_payment_method=pause` if going card-free | F-tiers-04, F-tiers-14, F-tiers-15, F-tiers-13, F-tiers-18 |
| 7 | Gate by at most four differences per step and copy the dynamic-pricing vendors' fences for the top tier: refresh frequency (nightly vs weekly), forecast horizon (e.g. 30 vs 90 days), history depth, and a named human review (quarterly pricing review), not only "AI" | Mohammed ≤4 attributes; RoomPriceGenie steps on 12→18-month horizon, 4x→24x daily uploads, 3-month→2-year history, dedicated revenue manager; Prisync gates the engine itself to Premium+; Shopify/Square put 24/7 phone support in the top tier | F-tiers-09, F-tiers-15, F-tiers-14, F-tiers-05, F-tiers-04 |
| 8 | Sign-in before pay: create the Floorline account (owner email + store name) first, then render the Pricing Table with `customer-session-client-secret`, or use Checkout directly and provision from `checkout.session.completed`; Link handles the card, not the account. Gate features with Entitlements `lookup_key`s `gallery_view` and `dynamic_pricing`, persisted locally; plan switching via Customer Portal "Switch plan" with proration on and downgrades at period end | Pricing Table cannot insert an account step; Claude and ChatGPT both sign in before plan choice; Entitlements webhook carries the full feature list; Portal "Switch plan" is "best when you have a good-better-best pricing model" | F-tiers-17, F-tiers-01, F-tiers-02, F-tiers-19, F-tiers-20, F-tiers-21 |
| 9 | CTA wording: "Start 30-day trial" on tiers 1–2, "Start trial" or "Talk to us" on tier 3 depending on whether the model needs onboarding data, "Talk to us" on multi-store; headline sells the outcome, not "Plans & Pricing" | Square "Try free for 30 days" / "Talk to our team"; Shopify "Start for free"; Claude "Try Claude"; Atlas: "Call us" not "Choose plan" for the sales tier, and "Plans & Pricing" is a weak headline | F-tiers-04, F-tiers-05, F-tiers-01, F-tiers-13 |

## Gaps and unverified
- OpenAI ChatGPT and Toast official pricing pages returned HTTP 403; tier prices come from two secondary sources each (Jun–Sep 2026). Layout details (badge, toggle, comparison table, CTA text) for ChatGPT are not verified. A browser session can close this gap in two minutes.
- "Sign-in before pay" for Claude and ChatGPT is stated from observed product behaviour, not from text on the pricing pages.
- Square's pricing page rendered without numbers; $89/location and the 30-day trial come from Square's features and help pages.
- Lightspeed monthly-billing rates and the Basic→Core gate detail come from NerdWallet, not the Lightspeed page, which lists Core and Plus with identical feature bullets.
- No primary ProfitWell/Price Intelligently, OpenView or a16z source on middle-tier share, tier ratios or "most popular" lift was found; everything on those points is secondary or a prevalence study. The HBR article is paywalled; Mohammed's ratio rules are from a Substack summary and Wikipedia.
- Clover tier names and prices conflict across three secondary sources; treat as indicative only.
- Duetto and IDeaS publish no prices; Duetto estimates ($200–500/property/month; $1,000/month start) are from a competitor blog and a review site. Omnia and Competera are quote-only. PriceLabs per-listing price is from G2, not fetched.
- Clientbook's ~$295/store on file is a quote; the public page shows no price.
- Furniture-vertical vendors with public tiers: none found (Furniture Wizard "upon request"; Frog, RetailVista, Myriad not found in one search pass).
- Not done in the time box: Toast IQ pricing confirmation, Lightspeed AI add-on pricing, Shopify POS Pro per-location vs plan mapping, a16z/HBR primary text.

## Sources
1. Pricing — Anthropic, 2026. https://claude.com/pricing
2. ChatGPT Pricing 2026: Free vs Go vs Plus vs Pro — CometAPI, updated 2026-09-03. https://www.cometapi.com/chatgpt-pricing-2026-free-vs-go-vs-plus-vs-pro/
3. ChatGPT pricing 2026 — eesel, 2026-09-09. https://eesel.ai/blog/chatgpt-pricing
4. ChatGPT pricing (official, 403 on fetch) — OpenAI. https://openai.com/chatgpt/pricing/
5. Retail POS pricing — Lightspeed, 2026. https://www.lightspeedhq.com/pos/retail/pricing/
6. Lightspeed Retail POS Review 2026 — NerdWallet. https://www.nerdwallet.com/reviews/small-business/lightspeed-retail-pos
7. Shopify pricing — Shopify, 2026. https://www.shopify.com/pricing
8. Square for Retail pricing — Square, 2026. https://squareup.com/us/en/point-of-sale/retail/pricing
9. Square for Retail features — Square, 2026. https://square.com/us/en/point-of-sale/retail/features
10. Square for Retail Plans (30-day trial) — Square help. https://squareup.com/help/au/article/6921
11. Restaurant POS pricing in 2026 — Katalyst, 2026-06-02 (corr. 2026-09-08). https://www.katalystos.com/blog/restaurant-pos-pricing-in-2026-real-costs-from-every-major-vendor
12. Clover POS Pricing Breakdown (2026) — UpMenu. https://www.upmenu.com/blog/clover-pos-pricing
13. Clientbook pricing plans — Clientbook, 2026. https://www.clientbook.com/pricing-plans
14. Clientbook Pricing Plans & History — PricingSaaS, 2026. https://pricingsaas.com/companies/clientbook
15. Furniture Wizard profile — Software Advice, 2026. https://www.softwareadvice.com/retail/furniture-wizard-profile
16. 5 Best Furniture Store Software — Fit Small Business, 2026. https://fitsmallbusiness.com/best-furniture-store-software/
17. The Good-Better-Best Approach to Pricing — Rafi Mohammed, HBR, Sep–Oct 2018. https://hbr.org/2018/09/the-good-better-best-approach-to-pricing
18. The Good-Better-Best Approach to Pricing (summary) — The Product Person, Substack. https://theproductperson.substack.com/p/the-good-better-best-approach-to
19. Good–better–best — Wikipedia. https://en.wikipedia.org/wiki/Good%E2%80%93better%E2%80%93best
20. What % of pricing pages highlight a 'Most popular' plan — Lazyweb Labs, July 2026. https://www.lazyweb.com/research/most-popular-badge-prevalence-pricing-pages
21. Does the three-tier pricing model still work in SaaS — Monetizely, 2026. https://www.getmonetizely.com/articles/good-better-best-does-the-three-tier-pricing-model-still-work-in-saas
22. What's the true cost of offering pre-pay discounts — SaaS Capital, 2014 survey. https://www.saas-capital.com/research/whats-the-true-cost-of-offering-pre-pay-discounts-to-saas-customers/
23. SaaS pricing guide — Stripe Atlas (Patrick McKenzie). https://stripe.com/guides/atlas/saas-pricing
24. SaaS pricing and packaging strategy — Stripe, 2026. https://stripe.com/resources/more/saas-pricing-and-packaging-strategy
25. Annual prepayment discount FAQ — Monetizely. https://www.getmonetizely.com/faqs/what-kind-of-discount-should-we-offer-for-annual-prepayment-versus-monthly-is-the-typical-approach-to-give-2-months-free-about-16-17-off-or-do-some-companies-do-a-different-discount-for-yearly-plans
26. Prisync pricing — Prisync, 2026. https://prisync.com/pricing/
27. RoomPriceGenie pricing — RoomPriceGenie, 2026. https://roompricegenie.com/pricing/
28. Duetto Gamechanger pricing — G2. https://www.g2.com/products/duetto/pricing
29. Duetto Pricing 2026 — RoomMaster (competitor blog). https://www.roommaster.com/blog/duetto-pricing
30. PriceLabs pricing — PriceLabs. https://hello.pricelabs.co/pricing/
31. Embeddable pricing table for subscriptions — Stripe Docs. https://docs.stripe.com/payments/checkout/pricing-table
32. Configure free trials for Checkout — Stripe Docs. https://docs.stripe.com/payments/checkout/free-trials
33. Configure the customer portal — Stripe Docs. https://docs.stripe.com/customer-management/configure-portal
34. Customer portal overview — Stripe Docs. https://docs.stripe.com/customer-management
35. Increase conversion and reduce costs with Link — Stripe Docs. https://docs.stripe.com/payments/link
36. Entitlements — Stripe Docs. https://docs.stripe.com/billing/entitlements
