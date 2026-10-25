# Existing tools: furniture POS/ERP, general POS, pricing software, and the negotiation-moment gap
Generated: 2026-10-24 · Agent: research-tools · Status: partial

Scope note: web search budget for the session ran out near the end; every row below has at least one vendor URL, but Clover's feature claims and a few prices rest on third-party pages and are marked "unconfirmed" or "third-party". Vendor pages that could not be fetched (403/JS-only) are named in Gaps.

## Summary
- The only shipping furniture system that lets an associate send a price override from the floor to an absent manager's phone, by text, with margin impact shown before approval, is STORIS NextGen Mobile POS, an enterprise ERP sold by quote to "more Top 100s than any other technology partner" (third-party estimates put it at roughly $200–500 per user per month plus setup; unverified) [F-tools-01].
- Every other furniture-specific system an independent can realistically buy (Furniture Wizard, Myriad PointCentric, PROFITsystems RETAILvantage, FROG, Genesis Advantage) stops at static permissions: role-based access, per-item dollar/percent discounting, profit/margin shown to whoever has rights, and nothing that computes a walk-away price or routes a live deal to the owner [F-tools-02, F-tools-03, F-tools-04, F-tools-05, F-tools-06].
- General POS used by small furniture stores (Shopify POS, Square for Retail, Lightspeed) offers a binary "manager PIN required to discount" and after-the-fact cost/margin reports; none offers a per-item minimum price, a percentage cap per role, an AI counteroffer, or remote approval from outside the store [F-tools-09, F-tools-10, F-tools-11, F-tools-12].
- Pricing-intelligence platforms (Prisync from $99/mo, Omnia SMB from EUR 399/mo, Competera, Pricefx, Wiser, Minderest, Intelligence Node) scrape online competitor prices for e-commerce catalogs; none is built for a 300-SKU showroom negotiation and none exposes a floor to a salesperson [F-tools-13].
- The closest analogs to a floor-side deal check with remote owner approval live outside furniture: Roadster Express Desking (car dealers, 2018; now CDK) lets a salesperson message terms to a desk manager who approves remotely while the salesperson stays with the customer; DealHub/Salesforce CPQ enforce per-SKU floors and tiered approvals for B2B SaaS at $150–200 per user per month; Odoo and NRS Plus sell $10–50 add-ons for per-user discount limits or remote manager override in generic POS [F-tools-14, F-tools-15, F-tools-16].
- Gap sentence for judges: "No product we could find gives an independent furniture store a per-item walk-away price computed from cost, age and delivery, a suggested counteroffer the salesperson can say out loud, and a one-tap approval on the owner's phone when the customer pushes below it; the only system with remote text approval at all is STORIS NextGen, an enterprise ERP priced and sold for Top-100 chains, and even it validates static discount rules rather than computing or explaining a floor." [F-tools-19]

## Findings

### F-tools-01 — STORIS NextGen Mobile POS already does remote manager override by text, with margin visibility, for enterprise furniture retailers
- **Value:** Vendor page (2026): "Associates can send a Manager Override Authorization Request directly to their manager's device for approval"; "Managers are conveniently alerted by a text message"; managers "can use visibility into how price adjustments impact margins to inform their decisions"; "STORIS will automatically validate that none of the core discounting rules the retailer sets have been broken" and "minimum requirements have been met to protect your margins". Managers can "manually override a price to match a competitor". STORIS claims "500+ retailers" and "More Top 100s Than Any Other Technology Partner". The 2015 release 9.6 added "advanced line item discounting" and "discount hierarchy configuration" (vendor claim via trade press). Pricing: quote only; ITQlick estimate ~$200–500/user/month, ~$25k–50k first year for 10 users (third-party, unverified); TrustRadius notes an entry-level setup fee.
- **Source:** [STORIS Mobile POS](https://www.storis.com/mobile-pos) — STORIS, 2026; [STORIS home](https://storis.com/) — STORIS, 2026; [STORIS releases 9.6](https://www.furnituretoday.com/business-news/storis-releases-9-6-version-of-selling-software) — Furniture Today, 2015-10-17; [STORIS pricing estimate](https://www.itqlick.com/storis-software/competitors) — ITQlick, undated (third-party)
- **Confidence:** high on features (vendor page quotes), low on price (third-party estimate; vendor publishes none)
- **Use:** pitch | submission-research

### F-tools-02 — Furniture Wizard shows profit/margin/markup at POS and prints "cost cyphers" on tags, but has no approval workflow or AI
- **Value:** Features page: "Instant calculations of profit, margin and markup" (POS); "Security will allow you to set permissions and restrict access to sensitive areas of the program"; tags can show "cost cyphers" (coded cost on the hangtag, the paper-era way to let staff see cost); iFurniture iPad app for associates. Serves "large and small furniture stores". No discount-approval, floor-price, or remote-approval feature described; no published price (Capterra: contact vendor, no free trial).
- **Source:** [Furniture Wizard features](https://furniturewizard.com/features/) — New Vision Information Systems, 2026; [Furniture Wizard mobile POS](https://furniturewizard.com/mobilepos/) — same; [Capterra listing](https://www.capterra.com/p/213321/Furniture-Wizard/) — Capterra, 2026
- **Confidence:** high (vendor page)
- **Use:** pitch | submission-research

### F-tools-03 — Myriad PointCentric targets single showrooms to ~12 stores; quoting with pricing on one screen, "approval tracking" in order management, no floor or margin control described
- **Value:** "Whether you're running one showroom or twelve"; segments include "Independent & Single-Location Retailers". Sales page: quotes and order entry cover "configurable products, pricing, financing, deposits"; order management includes approval tracking (order progress, not price approval). No discount limits, margin visibility at POS, or mobile approval described. Pricing not published (demo/quote). Trade press (2005): customers $2M–$70M annual sales.
- **Source:** [Myriad Who We Serve](https://myriadsoftware.com/who-we-serve/) — Myriad Software, 2026; [Myriad Sales](https://myriadsoftware.com/sales/) — Myriad Software, 2026; [Myriad conference](https://www.furnituretoday.com/business-news/retailers-learn-20th-annual-myriad-conference) — Furniture Today (older)
- **Confidence:** medium (vendor pages thin; absence of a feature on a page is not proof of absence in product)
- **Use:** submission-research

### F-tools-04 — PROFITsystems RETAILvantage: per-item $/% discounting plus field-level privilege levels; no remote approval; quote pricing
- **Value:** POS page: "Dollar or percentage discounting per item"; passwords and privilege levels "for pages, buttons, and fields"; change tracking (who/when); sales entered "from the sales floor or the back office". Historic positioning: retailers with $1M–$80M sales (2013 trade press). Pricing not published. Owned by HighJump (Körber) since 2014.
- **Source:** [PROFITsystems POS](https://www.profitsystems.com/find-your-fit/point-of-sale-system-pos/) — PROFITsystems, 2026; [PROFITsystems home](https://www.profitsystems.com/) — 2026; [Nationwide teams with ProfitSystems](https://www.furnituretoday.com/business-news/nationwide-teams-with-profitsystems-for-group-program) — Furniture Today, 2013
- **Confidence:** high on listed features, medium on segment (old press)
- **Use:** submission-research

### F-tools-05 — FROG (Furniture Retail Operations Group, furnguy.com): web/mobile app for order entry; pricing "a fraction of what our competitors charge" but unpublished; no discount or margin controls described
- **Value:** "The FROG App can run on any web or mobile device and offers most of the functionality from the Windows retail software"; features listed: Sales Entry, Item Lookup, Associate Tracker, dashboards with "Detailed salesperson analysis". No discount approval, floor, or margin-at-POS feature on vendor pages. Reviews (TrustRadius/Capterra) call the UI dated and reporting hard without custom work. frogpos.com is a parked domain; vendor site is furnguy.com.
- **Source:** [FROG home](https://www.furnguy.com/) — Furniture Retail Operations Group, 2026; [FROG App](https://www.furnguy.com/services/frog-app) — same; [FROG on G2 pricing](https://www.g2.com/products/furniture-retail-operations-group-frog/pricing) — G2 (no price listed)
- **Confidence:** medium
- **Use:** submission-research

### F-tools-06 — Genesis Advantage (Genesis Software Systems): on-premise Windows inventory/accounting for small-to-mid furniture retailers; vendor site not found; quote pricing
- **Value:** Directory listings only: "inventory control and accounting software designed specifically for furniture retailers"; Capterra: pricing per feature, contact vendor. GERS (the 1990s–2000s "largest provider" for furniture) is a different, legacy enterprise lineage; no current product page found. Feature claims on discounts/margins: unconfirmed.
- **Source:** [Genesis Advantage on Capterra](https://www.capterra.com/p/126875/Genesis-Advantage/) — Capterra, 2026; [Serchen listing](https://serchen.com/company/genesis-advantage) — Serchen; [GERS set to introduce POS](https://www.furnituretoday.com/business-news/gers-set-to-introduce-pos-system-next-year/) — Furniture Today, 2001
- **Confidence:** low (no vendor page reachable)
- **Use:** submission-research

### F-tools-07 — RetailVista, Bravo Business Media, iDeal, Furniture Hub and DealerChoice are not US independent-furniture POS competitors
- **Value:** RetailVista is NedFox (Netherlands/UK) cloud POS/ERP for garden centres, pet, DIY and thrift; furniture is not mentioned on its site; Valsoft acquired NedFox in April 2026. Bravo Business Media is "a retail-focused eCatalog service to the decorative showroom industry" (600+ showrooms), acquired by Unilog in Feb 2021; it is B2B catalog/e-commerce, not POS. "iDeal", "Furniture Hub" and "DealerChoice" returned no furniture-retail product in any search (the only DealerChoice hit is an Oxlo Systems auto-dealer program; contract-furniture dealer ERPs are ECI TeamDesign and similar). Mark as not found.
- **Source:** [RetailVista](https://retailvista.io/en/) — NedFox, 2026; [Valsoft acquires NedFox](https://www.newswire.com/news/valsoft-corporation-strengthens-its-retail-software-portfolio-with-the) — Newswire, 2026; [Unilog acquires Bravo Business Media](https://salestechstar.com/sales-marketing/b2b-ecommerce-leader-unilog-acquires-bravo-business-media/) — SalesTechStar, 2021-02-18; [ECI office furniture ERP](https://ecisolutions.com/industries/office-furniture) — ECI, 2026
- **Confidence:** high for RetailVista/Bravo; medium for "not found" (name may be misspelled or regional)
- **Use:** submission-research

### F-tools-08 — Clientbook is a clienteling CRM (~$295/month, third-party figure) with AI product recommendations, not a pricing or approval tool
- **Value:** Vendor pricing page lists no numbers ("Plans for every business, every budget", quote after demo). Software Advice/SoftwareFinder list Signature/Elite/Premium at $295/month each (third-party, "subject to change"). Industries: jewelry, furniture, fashion, music. Features: client management, messaging, automations, AI insights, product recommendations, sales associate tracking. Nothing on discounts, margins or price approval.
- **Source:** [Clientbook pricing plans](https://www.clientbook.com/pricing-plans) — Clientbook, 2026; [SoftwareFinder Clientbook](https://softwarefinder.com/crm/clientbook) — SoftwareFinder (third-party)
- **Confidence:** medium (price third-party)
- **Use:** submission-research | pitch

### F-tools-09 — Shopify POS: discount permission is allowed / denied / approval-required (manager PIN); no percentage cap; profit reports use cost per item; POS Pro $89 per location per month
- **Value:** POS permissions page, "Apply custom discounts": "Allowed, which lets staff apply custom discounts"; "Denied, which restricts staff from applying custom discounts"; "Approval required, which requires staff with manager approval and apply discount permissions allowed to enter their PIN". No price-override permission, no cost-visibility permission, no percentage cap on the page. Profit reports: gross profit "calculated by subtracting the cost from net sales", gross margin "([net sales - cost] / net sales) * 100", per product/variant/POS location, only for items with a recorded cost per item. POS Pro: "$89 USD/month billed yearly for each location", includes staff roles and permissions. Approval is a PIN typed on the same device: the manager must be physically present.
- **Source:** [Shopify POS permissions](https://help.shopify.com/en/manual/your-account/users/roles/permissions/pos-permissions) — Shopify Help Center, 2026; [Shopify profit reports](https://help.shopify.com/en/manual/reports-and-analytics/shopify-reports/report-types/default-reports/profit-reports) — Shopify Help Center, 2026; [Shopify POS pricing](https://www.shopify.com/pos/pricing) — Shopify, 2026
- **Confidence:** high
- **Use:** pitch | submission-research

### F-tools-10 — Square for Retail: unit costs and "COGS and Margin" / "Projected Profit" reports need the Plus plan; discounts can be passcode-restricted; no floor price, no remote approval
- **Value:** Retail pricing page: Plus includes "Cost of goods sold and inventory reporting"; "Manage unit costs" lets you add unit costs "to better calculate margins"; tiers Free / Plus / Premium / Square Pro (custom, >$250k/yr processing). Help: "To view the COGS and Margin report, Projected Profit report ... you will need to have a subscription to Square for Retail Plus"; staff need explicit permissions to view COGS reports. Team permission "Apply Restricted Discounts and Comps to a Transaction" unlocks passcode-protected discounts (4-digit passcode entered at the register); Retail Plus includes two custom permission sets, Advanced Access unlimited. Plus list price not readable from the vendor page in this session; third-party guides cite $89/month per location (unconfirmed).
- **Source:** [Square for Retail pricing](https://squareup.com/us/en/point-of-sale/retail/pricing) — Square, 2026; [Square COGS help](https://squareup.com/help/us/en/article/8522-track-cost-of-goods-sold) — Square, 2026; [Square apply discounts](https://squareup.com/help/us/en/article/5362-apply-discounts) — Square, 2026; [Square team permissions](https://squareup.com/help/us/en/article/5822) — Square, 2026
- **Confidence:** high on features, medium on price
- **Use:** pitch | submission-research

### F-tools-11 — Lightspeed Retail: $89 / $149 / $289 per month; custom user roles and landed-cost margins on all plans; "Requires manager" code for a discount; margin by employee only in after-the-fact reports
- **Value:** Pricing page (X-Series): Basic $89/mo, Core $149/mo, Plus $289/mo ("save up to 18%" annual); all plans include "Custom User Roles" and "Landed Costs ... get more accurate margins". Discount setup (ShopKeep/Lightspeed Retail support): "Check this box to require a manager code before a cashier can apply the discount"; at the register "have a manager enter their register code and tap Verify". Line Employee report shows "total sales, discounts, and cost by employee" so an owner can find underpriced items after the sale. No per-item floor, no percentage cap per role found, approval requires the manager at the register.
- **Source:** [Lightspeed Retail pricing](https://www.lightspeedhq.com/pos/retail/pricing/) — Lightspeed, 2026; [Lightspeed discounts (ShopKeep support)](https://shopkeep-support.lightspeedhq.com/support/backoffice/discounts) — Lightspeed, 2026; [Sales by employee](https://shopkeep-support.lightspeedhq.com/support/reporting/sales-by-employee) — Lightspeed, 2026
- **Confidence:** high
- **Use:** pitch | submission-research

### F-tools-12 — Clover: roles Admin / Manager / Employee / custom; discount and item-cost controls unconfirmed on vendor pages (JS-only site, search budget exhausted)
- **Value:** Third-party guides: permission levels Admin, Manager, Employee, custom roles; refunds restrictable by role; nothing found on discount caps, manager approval for discounts, or item cost/margin reporting. Clover's pricing and retail pages returned only a title to the fetcher. Treat all Clover feature cells as unconfirmed; price unknown (quote via merchant services reseller).
- **Source:** [Clover home](https://www.clover.com/pricing) — Clover, 2026 (not parseable); [Clover best practices guide](https://help.clubspeed.com/clubspeed-knowledge-center/clover-best-practices-guide) — Clubspeed (third-party); [Clover partner POS guide](https://partners.letsgetoffline.com/article/117-pos-guide-clover) — Offline (third-party)
- **Confidence:** low
- **Use:** submission-research

### F-tools-13 — Pricing-intelligence platforms are online competitor-scraping tools priced from $99/month (Prisync) to six figures (Pricefx); none is built for a showroom negotiation and none exposes a floor to floor staff
- **Value:** Prisync: URL-based plans $99 (100 products), $199 (1,000), $399 (5,000) per month; channel/hybrid up to $799. Omnia Retail: SMB "Starting at EUR 399 per month", single shop, up to 5 users; Enterprise custom. Pricefx: "Enterprise Pricing Intelligence Platform", no public price, customers like Ford (2.5M parts); third-party cites ~$100k/yr. Competera: "Pricing AI solutions for enterprise retail", "Trusted by 50+ retailers", no public price. Minderest: "11 of the world's 50 largest retailers", online sources, no price. Wiser: 300+ brands/retailers, Price/Market/MAP Intelligence, online and marketplace focus, no price. Intelligence Node: "Fortune 1000 brands and retailers", lists "Furniture & Home Decor" as an industry, no price. No evidence any is used by small brick-and-mortar furniture stores; all assume an online catalog with matchable competitor URLs.
- **Source:** [Prisync pricing](https://prisync.com/pricing/) — Prisync, 2026; [Omnia pricing](https://www.omniaretail.com/pricing) — Omnia Retail, 2026; [Pricefx pricing](https://www.pricefx.com/pricing/) — Pricefx, 2026; [Competera](https://competera.ai/) — Competera, 2026; [Minderest](https://www.minderest.com/) — Minderest, 2026; [Wiser](https://www.wiser.com/) — Wiser Solutions, 2026; [Intelligence Node](https://www.intelligencenode.com/) — Intelligence Node, 2026; [Pricefx cost comparison](https://www.selecthub.com/pricing-software/competera-vs-pricefx) — SelectHub (third-party)
- **Confidence:** high on published prices, medium on "not used by small furniture stores" (absence of evidence)
- **Use:** pitch | submission-research

### F-tools-14 — B2B deal desk / CPQ enforce per-SKU floors and tiered approvals, but for SaaS sales teams at $150–200 per user per month
- **Value:** DealHub community example: "rather than approving based on a discount percentage, TechNest sets absolute floor prices per SKU"; "Sales Reps must not go below $80, and Managers must not approve less than $70" on a $100 list; built with product attributes + general workflows because "DealHub's standard approval workflows rely on discount percentage thresholds". DealHub pricing: "Request Pricing", "Built for SaaS and Services revenue teams". DealHub glossary: tiered approval, e.g. "a 10% discount needing sales manager approval, while a 25% discount requires the VP of Sales". Salesforce Revenue Cloud: Growth $150/user/month, Advanced $200/user/month, annual contract; Advanced Approvals emails approvers and reads the reply as approve/reject. Vendavo/Zilliant/PROS offer deal guidance with margin floors for distributors (third-party descriptions only).
- **Source:** [DealHub floor pricing](https://circle.dealhub.io/cpq-7/configuring-floor-pricing-170) — DealHub Community, 2025; [DealHub discount approval glossary](https://dealhub.io/glossary/discount-approval/) — DealHub, 2026; [DealHub pricing](https://dealhub.io/pricing/) — DealHub, 2026; [Salesforce Revenue Cloud pricing](https://www.salesforce.com/sales/cpq/pricing/) — Salesforce, 2026; [Advanced Approvals Trailhead](https://trailhead.salesforce.com/content/learn/modules/advanced-approvals-for-sales-reps-and-approval-managers/manage-approval-submissions-and-responses) — Salesforce, 2026
- **Confidence:** high
- **Use:** pitch | layer1-spec

### F-tools-15 — Closest workflow analog: Roadster Express Desking (car dealers, 2018; CDK since 2021) lets the salesperson message terms to a desk manager who approves remotely while staying with the customer
- **Value:** "All custom payments, non-standard terms, rate overrides or bonus discount additions can be approved by desk managers remotely while the sales agent remains with the guest"; the manager "is able to review the terms, unlock codes, override the deal if necessary and grant approval", including from a mobile device. Launched Oct 8, 2018 inside Roadster Express Storefront; CDK Global acquired Roadster June 2, 2021. CDK's own buying guide asks for desking that "works from the parking lot". vAuto (Cox) is appraisal/market pricing ("Predictive & Dynamic Pricing"), mobile only for reconditioning approvals; no salesperson floor or desking approval on its site. Pricing for all: dealer quote.
- **Source:** [Roadster Express Desking](https://www.autoremarketing.com/ar/technology/roadster-aims-smooth-out-salesperson-desk-manager-communication/) — Auto Remarketing, 2018-10-08; [CDK acquires Roadster](https://www.cbtnews.com/cdk-global-enters-digital-retailing-with-roadster-acquisition/) — CBT News, 2021-06-02; [CDK choosing a desking provider](https://cdkglobal.com/insights/read-choosing-desking-provider) — CDK, 2021; [vAuto](https://www.vauto.com/) — Cox Automotive, 2026
- **Confidence:** high
- **Use:** pitch | submission-research

### F-tools-16 — Generic POS add-ons sell the pieces separately: per-user discount limits with manager approval (Odoo, ~$50 one-time), remote manager override from a merchant app (NRS Plus, $9.95/mo add-on), online margin-floor discount blocking (Profit Guard for Shopify, $0–29.99/mo)
- **Value:** Odoo "POS Discount Approval Fixed Limit": "Define user-specific discount limits (cash amount & percentage)"; above the limit a request goes to a manager and "Until approval is granted, the POS order cannot be validated"; $50.10 (v18). NRS Plus (bodega/convenience POS): "Approve critical POS actions remotely with your merchant app; from anywhere, anytime" — $9.95/mo add-on on Basic ($19.95/mo), included on Pro $34.95+. Profit Guard (Shopify app, HN Studio): checks each discount against margin rules, can disable or reduce it; Free / $19.99 / $29.99 per month; Shopify Admin/online discounts, POS support not stated. None combines per-item cost-based floor + negotiation guidance + owner phone approval, and none is furniture-aware (age, delivery, floor-sample status).
- **Source:** [Odoo discount approval module](https://apps.odoo.com/apps/modules/18.0/deckspectra_pos_disc_approval_fixed_limit) — Odoo Apps, 2026; [NRS Plus pricing](https://nrsplus.com/pricing/) — National Retail Solutions, 2026; [NRS Plus home](https://nrsplus.com/) — NRS, 2026; [Profit Guard](https://apps.shopify.com/profit-gaurd) — Shopify App Store, 2026
- **Confidence:** high
- **Use:** pitch | submission-research

### F-tools-17 — Customer-facing AI haggling bots exist online only (Nibble $499/mo + 2% above $24,950 sales; BargainIt), with furniture e-commerce clients; none runs on a showroom floor between a human salesperson and a human customer
- **Value:** Nibble Shopify listing: "$499 / month" + "2% on sales above $24,950"; AI chatbot "discovers the deal your customer needs" within discounts the merchant sets; triggers are dwell time, exit intent, email; integration is online checkout. Nibble cites furniture clients (Industry West; Eve Sleep mattress example in Fortune, 2024). BargainIt (Shopify) offers "store-approved" counteroffers from margins and discount rules. These negotiate with the shopper, replacing the salesperson; they do not coach a salesperson or ask an owner.
- **Source:** [Nibble on Shopify](https://apps.shopify.com/nibble-chat-bot) — Shopify App Store, 2026; [Nibble on BigCommerce](https://bigcommerce.com/apps/nibble-ai-negotiation) — BigCommerce, 2026; [Negotiating chatbot Nibble](https://www.fortune.com/2024/07/16/negotiating-chatbot-nibble-ai-ecommerce) — Fortune, 2024-07-16; [BargainIt](https://apps.shopify.com/bargainit) — Shopify App Store, 2026
- **Confidence:** high
- **Use:** pitch

### F-tools-18 — Electronic shelf labels cost roughly $5–20 per tag plus a $300–400 gateway and ~$500 software (plus SaaS); furniture adoption is limited to giants (Nebraska Furniture Mart, ~30,000 tags, 2014) and pilots (Möbel Heinrich accessories area, 2025)
- **Value:** KORONA POS guide (2026-09-17): labels "$5 to over $20" (average $5–12), gateways "$300-$400", management software "about $500 upfront" plus monthly SaaS; worth it "for shops with many products whose prices change often". Pricer case: NFM, three stores, ~30,000 graphic ESLs, driven by nightly electronics price matching and 600 paper labels a day; it "planned to extend the system to its furniture department". VusionGroup/Möbel Heinrich: pilot limited to the decor/accessories area "to determine customer acceptance and user-friendliness". Why small furniture stores rarely adopt: a showroom has a few hundred large items, prices change seasonally not daily, the tag price is the opening bid in a negotiation not the transaction price, and a $2–6k pilot buys nothing a printed hangtag with a cost cypher does not already do. Vendor pricing for Pricer/VusionGroup/Hanshow is quote-only (not found).
- **Source:** [How much do ESLs cost](https://koronapos.com/blog/how-much-do-electronic-shelf-labels-cost/) — KORONA POS, 2026-09-17; [Nebraska Furniture Mart and Pricer](https://pricer.com/blog/nebraska-furniture-mart) — Pricer, 2014-02-05; [Möbel Heinrich pilots VusionGroup ESLs](https://retail-optimiser.de/en/?p=21251) — Retail Optimiser, 2025-03-12
- **Confidence:** medium (cost figures are vendor-blog ranges; adoption reasoning is inference)
- **Use:** submission-research

### F-tools-19 — No product found that gives an independent brick-and-mortar store a per-item minimum acceptable price with owner approval at the moment of negotiation
- **Value:** Searched: "negotiation guardrail", "price floor" + salesperson + owner approval, "discount authority" apps, startup/Product Hunt/YC angles, furniture/mattress/jewelry verticals, retail CPQ. Results: B2B deal desks (DealHub, Salesforce, Vendavo, Zilliant, PROS), car-dealer desking (Roadster), generic POS add-ons (Odoo, NRS Plus), online haggle bots (Nibble, BargainIt), a hobby GitHub issue describing owner approval with web push. The one furniture-native remote approval is STORIS NextGen (enterprise, quote-priced). None of these: (a) computes a per-item floor from cost, age, floor-sample status and delivery; (b) suggests a counteroffer the salesperson can say; (c) routes to the owner's phone in one tap; (d) is priced for a one- to three-store independent. Stated clearly: none found.
- **Source:** [DealHub floor pricing](https://circle.dealhub.io/cpq-7/configuring-floor-pricing-170); [STORIS Mobile POS](https://www.storis.com/mobile-pos); [NRS Plus](https://nrsplus.com/); [shopkeeper issue #45 (hobby project)](https://github.com/humberto0/shopkeeper/issues/45) — GitHub, 2025
- **Confidence:** medium (absence of evidence after ~45 searches; web search budget exhausted before a final sweep of Product Hunt / Crunchbase)
- **Use:** pitch | submission-research

## Tables

### Comparison matrix

Legend: Y = confirmed on vendor page; N = vendor page describes the feature set and this is absent; U = unconfirmed (no vendor evidence either way); "PIN" = manager must be physically at the device.

| Tool | Segment | Per-item cost & margin visible to floor staff? | Min-price / discount-approval rule? | Floor-side mobile deal check? | AI price suggestion? | Owner remote approval? | Price (USD/mo or setup) | Source |
|---|---|---|---|---|---|---|---|---|
| STORIS (NextGen Mobile POS) | Furniture ERP, Top-100 chains to mid-size | Managers see margin impact of a price change (Y); associates: U | Y: static discount rules + minimum requirements validated; manager override to match competitor | Y: cart, quote, discounting on any device | N | Y: "Manager Override Authorization Request" to manager's device, text alert | Quote; third-party est. $200–500/user/mo + setup | storis.com/mobile-pos |
| Furniture Wizard | Furniture POS, small to large independents | Y: "Instant calculations of profit, margin and markup" at POS; "cost cyphers" on tags (permission-gated) | U: role permissions only, no floor rule described | Partial: iFurniture iPad app (room packages, upsell prompts) | N | N | Quote (no published price) | furniturewizard.com/features |
| Myriad PointCentric | Furniture ERP, 1–12 showrooms | U | N (approval tracking is order status) | Partial: tablet inventory lookup | N | N | Quote | myriadsoftware.com |
| PROFITsystems RETAILvantage | Furniture ERP, ~$1M–$80M retailers | U (field-level privileges can hide cost) | Partial: per-item $/% discount with privilege levels; no floor | Partial: sales entry from floor | N | N | Quote | profitsystems.com |
| FROG (furnguy.com) | Furniture POS, budget tier | U | U | Y: FROG App on any device (sales entry, item lookup) | N | N | Quote ("fraction of competitors") | furnguy.com |
| Genesis Advantage | Furniture back office, small-mid, on-prem | U | U | N | N | N | Quote | capterra.com (vendor site not found) |
| Clientbook | Clienteling CRM (jewelry, furniture) | N (CRM) | N | Partial: associate app, no pricing | Y for product recommendations, not price | N | ~$295/mo (third-party) | clientbook.com/pricing-plans |
| Shopify POS Pro | General POS | Cost per item in admin; profit reports; staff visibility U | Partial: "Apply custom discounts" allowed / denied / approval required (manager PIN); no % cap, no floor | Y (POS app) | N | N (PIN on device) | $89/location/mo + Shopify plan | help.shopify.com pos-permissions |
| Square for Retail | General POS | Unit costs + "COGS and Margin" report on Plus; permission-gated, back-office | Partial: passcode-restricted discounts; no % cap, no floor | Y (POS app) | N | N (4-digit passcode on device) | Free; Plus ~$89/location/mo (third-party); Premium custom | squareup.com/us/en/point-of-sale/retail/pricing |
| Lightspeed Retail (X-Series) | General POS | Landed-cost margins; cost/profit by employee in reports (after sale) | Partial: "Requires manager" code per discount; custom roles; no % cap, no floor | Y (iPad POS) | N | N (manager code at register) | $89 / $149 / $289 per mo | lightspeedhq.com/pos/retail/pricing |
| Clover | General POS | U | U (roles Admin/Manager/Employee per third party) | Y (handheld devices) | N | U | Unknown (reseller quote) | clover.com (unparseable); third-party |
| Prisync | Online price tracking | N | N | N | Repricing rules (not AI) | N | $99–$799/mo | prisync.com/pricing |
| Omnia Retail | Online pricing, SMB to enterprise | N | N | N | Y (dynamic pricing) | N | From EUR 399/mo | omniaretail.com/pricing |
| Competera / Pricefx / Wiser / Minderest / Intelligence Node | Enterprise pricing intelligence | N | N | N | Y (enterprise price optimization) | N | Quote; Pricefx ~$100k/yr (third-party) | vendor homepages |
| DealHub CPQ | B2B SaaS deal desk | Rep sees net price vs floor attribute (configured) | Y: per-SKU floor (rep $80 / manager $70 example) via workflows | N (desk, not floor) | N | Y: approval workflow routed to approver (email/app) | Quote | circle.dealhub.io floor pricing |
| Salesforce Revenue Cloud / CPQ Advanced Approvals | B2B enterprise CPQ | Configurable | Y: discount-threshold rules, tiered approvers | N | Partial (Einstein, add-on) | Y: approve by email reply | $150–$200/user/mo, annual | salesforce.com/sales/cpq/pricing |
| Roadster Express Desking (CDK) | Car dealer desking | Manager sees deal; salesperson sees payments | Y: non-standard terms need desk manager | Y: salesperson stays with guest | N | Y: desk manager approves remotely, mobile | Dealer quote | autoremarketing.com 2018 |
| vAuto (Cox) | Car dealer inventory pricing | Dealer-side only | N | N | Y: market-based pricing | N | Dealer quote | vauto.com |
| Odoo POS discount-limit module | Generic POS add-on | N | Y: per-user % and cash limits; order blocked until manager approves | Y (Odoo POS) | N | U (approval location not stated) | ~$50 one-time + Odoo | apps.odoo.com |
| NRS Plus Remote Manager Override | Convenience-store POS | N | Partial: critical actions gated | Y (register) | N | Y: from merchant app "anywhere, anytime" | $9.95/mo add-on (Basic $19.95/mo) | nrsplus.com/pricing |
| Nibble / BargainIt | Online haggle chatbot | N (talks to shopper) | Y: merchant-set discount limits | N (web only) | Y: AI negotiation with shopper | N | Nibble $499/mo + 2% above $24,950 | apps.shopify.com |
| Profit Guard (Shopify app) | Online discount guard | N | Y: min-margin rule blocks/reduces discounts | N (admin/online) | Partial: AI suggestions on Pro | N | $0 / $19.99 / $29.99 per mo | apps.shopify.com/profit-gaurd |
| Pricer / VusionGroup / Hanshow ESL | Shelf-label hardware | Shows price, not cost | N | N | N | N | ~$5–20/tag + $300–400 gateway + software | koronapos.com; pricer.com |

### What exists vs what the moment needs

| Need at the negotiation moment (owner away) | Who covers it today | Gap |
|---|---|---|
| Salesperson sees this item's true floor (cost + age + floor-sample + delivery) | Nobody per item; Furniture Wizard shows margin math, STORIS validates static rules | No cost-derived floor anywhere |
| A counteroffer the salesperson can say | Nibble says it to the shopper online; nothing for a human salesperson in-store | None |
| Owner approves from a phone in seconds | STORIS NextGen (text), Roadster (cars), NRS Plus (bodegas) | None for independent furniture at SMB price |
| Explanation of why the floor is what it is | DealHub shows a floor-difference number; no narrative anywhere | None |
| Price under $100/mo, no ERP migration | Shopify/Square/Lightspeed tiers, Odoo/NRS add-ons | They lack the floor and approval logic |

## Gaps and unverified
- Clover: vendor pricing/retail/help pages returned only a title to the fetcher and the session's web-search budget ran out; all Clover cells are unconfirmed.
- Square for Retail Plus list price could not be read from the vendor page (template placeholders); ~$89/location/mo is from third-party guides.
- STORIS price is a third-party estimate (ITQlick); STORIS publishes none. STORIS NextGen target size (minimum revenue) is not stated by the vendor.
- Genesis Software Systems has no reachable vendor site; Capterra/Serchen listings only. GERS lineage not traced to a current product.
- "iDeal", "Furniture Hub", "DealerChoice" not found as furniture-retail POS products after several name variants; could be regional, renamed, or misremembered.
- Furniture Wizard, Myriad, PROFITsystems, FROG: absence of floor-price or remote-approval features is inferred from vendor feature pages; a demo could reveal unlisted settings. Marked "U" where the page is silent.
- TrustRadius, Capterra, Software Advice, Unilog, and Nibble's own pricing page returned 403/404; third-party figures used instead are labeled.
- Pricer / VusionGroup / Hanshow per-tag list prices not published; ESL cost ranges are from a POS vendor's blog and a 2014 ABI figure.
- Pricing-intelligence vendors: "not used by small brick-and-mortar furniture stores" is absence of evidence (no case study or SMB plan found), not a measured share.
- Final sweep of Product Hunt / Crunchbase / YC directory for a "negotiation guardrail" startup was not completed (search budget); recommend one more pass before the pitch is locked.
- Not covered: Ordorite, RetailSystem (Furniture First partner), LS Retail, Microsoft Dynamics (LS Central has per-role maximum discount %); all enterprise-tier or non-US; none changes the gap.

## Sources
1. STORIS Mobile POS — STORIS, 2026 — https://www.storis.com/mobile-pos
2. STORIS home (500+ retailers, Top 100s) — STORIS, 2026 — https://storis.com/
3. STORIS releases 9.6 version of selling software — Furniture Today, 2015-10-17 — https://www.furnituretoday.com/business-news/storis-releases-9-6-version-of-selling-software
4. STORIS pricing estimate — ITQlick (third-party), undated — https://www.itqlick.com/storis-software/competitors
5. Furniture Wizard features — New Vision Information Systems, 2026 — https://furniturewizard.com/features/
6. Furniture Wizard mobile POS (iFurniture) — 2026 — https://furniturewizard.com/mobilepos/
7. Furniture Wizard on Capterra — Capterra, 2026 — https://www.capterra.com/p/213321/Furniture-Wizard/
8. Myriad Who We Serve — Myriad Software, 2026 — https://myriadsoftware.com/who-we-serve/
9. Myriad Sales — Myriad Software, 2026 — https://myriadsoftware.com/sales/
10. PROFITsystems POS — PROFITsystems, 2026 — https://www.profitsystems.com/find-your-fit/point-of-sale-system-pos/
11. PROFITsystems home — 2026 — https://www.profitsystems.com/
12. Nationwide teams with ProfitSystems — Furniture Today, 2013 — https://www.furnituretoday.com/business-news/nationwide-teams-with-profitsystems-for-group-program
13. FROG home — Furniture Retail Operations Group, 2026 — https://www.furnguy.com/
14. FROG App — 2026 — https://www.furnguy.com/services/frog-app
15. FROG pricing on G2 — G2, 2026 — https://www.g2.com/products/furniture-retail-operations-group-frog/pricing
16. Genesis Advantage — Capterra, 2026 — https://www.capterra.com/p/126875/Genesis-Advantage/
17. Genesis Advantage — Serchen — https://serchen.com/company/genesis-advantage
18. GERS set to introduce POS system — Furniture Today, 2001 — https://www.furnituretoday.com/business-news/gers-set-to-introduce-pos-system-next-year/
19. RetailVista — NedFox, 2026 — https://retailvista.io/en/
20. Valsoft acquires NedFox — Newswire, 2026 — https://www.newswire.com/news/valsoft-corporation-strengthens-its-retail-software-portfolio-with-the
21. Unilog acquires Bravo Business Media — SalesTechStar, 2021-02-18 — https://salestechstar.com/sales-marketing/b2b-ecommerce-leader-unilog-acquires-bravo-business-media/
22. ECI office furniture dealer ERP — ECI, 2026 — https://ecisolutions.com/industries/office-furniture
23. Clientbook pricing plans — Clientbook, 2026 — https://www.clientbook.com/pricing-plans
24. Clientbook pricing — SoftwareFinder (third-party) — https://softwarefinder.com/crm/clientbook
25. Shopify POS permissions — Shopify Help Center, 2026 — https://help.shopify.com/en/manual/your-account/users/roles/permissions/pos-permissions
26. Shopify profit reports — Shopify Help Center, 2026 — https://help.shopify.com/en/manual/reports-and-analytics/shopify-reports/report-types/default-reports/profit-reports
27. Shopify POS pricing — Shopify, 2026 — https://www.shopify.com/pos/pricing
28. Square for Retail pricing — Square, 2026 — https://squareup.com/us/en/point-of-sale/retail/pricing
29. Square track cost of goods sold — Square, 2026 — https://squareup.com/help/us/en/article/8522-track-cost-of-goods-sold
30. Square apply discounts — Square, 2026 — https://squareup.com/help/us/en/article/5362-apply-discounts
31. Square team permissions — Square, 2026 — https://squareup.com/help/us/en/article/5822
32. Lightspeed Retail pricing — Lightspeed, 2026 — https://www.lightspeedhq.com/pos/retail/pricing/
33. Lightspeed Retail discounts (requires manager) — Lightspeed support, 2026 — https://shopkeep-support.lightspeedhq.com/support/backoffice/discounts
34. Lightspeed sales by employee — Lightspeed support, 2026 — https://shopkeep-support.lightspeedhq.com/support/reporting/sales-by-employee
35. Clover pricing (unparseable) — Clover, 2026 — https://www.clover.com/pricing
36. Clover best practices guide — Clubspeed (third-party) — https://help.clubspeed.com/clubspeed-knowledge-center/clover-best-practices-guide
37. Prisync pricing — Prisync, 2026 — https://prisync.com/pricing/
38. Omnia Retail pricing — Omnia, 2026 — https://www.omniaretail.com/pricing
39. Pricefx pricing — Pricefx, 2026 — https://www.pricefx.com/pricing/
40. Competera — 2026 — https://competera.ai/
41. Minderest — 2026 — https://www.minderest.com/
42. Wiser Solutions — 2026 — https://www.wiser.com/
43. Intelligence Node — 2026 — https://www.intelligencenode.com/
44. Competera vs Pricefx cost — SelectHub (third-party) — https://www.selecthub.com/pricing-software/competera-vs-pricefx
45. Configuring floor pricing — DealHub Community, 2025 — https://circle.dealhub.io/cpq-7/configuring-floor-pricing-170
46. Discount approval glossary — DealHub, 2026 — https://dealhub.io/glossary/discount-approval/
47. DealHub pricing — DealHub, 2026 — https://dealhub.io/pricing/
48. Salesforce Revenue Cloud pricing — Salesforce, 2026 — https://www.salesforce.com/sales/cpq/pricing/
49. Advanced Approvals, manage submissions — Salesforce Trailhead, 2026 — https://trailhead.salesforce.com/content/learn/modules/advanced-approvals-for-sales-reps-and-approval-managers/manage-approval-submissions-and-responses
50. Roadster Express Desking — Auto Remarketing, 2018-10-08 — https://www.autoremarketing.com/ar/technology/roadster-aims-smooth-out-salesperson-desk-manager-communication/
51. CDK acquires Roadster — CBT News, 2021-06-02 — https://www.cbtnews.com/cdk-global-enters-digital-retailing-with-roadster-acquisition/
52. Choosing a desking provider — CDK Global, 2021 — https://cdkglobal.com/insights/read-choosing-desking-provider
53. vAuto — Cox Automotive, 2026 — https://www.vauto.com/
54. POS Discount Approval Fixed Limit — Odoo Apps, 2026 — https://apps.odoo.com/apps/modules/18.0/deckspectra_pos_disc_approval_fixed_limit
55. NRS Plus pricing — National Retail Solutions, 2026 — https://nrsplus.com/pricing/
56. NRS Plus home (Remote Manager Override) — 2026 — https://nrsplus.com/
57. Profit Guard — Shopify App Store, 2026 — https://apps.shopify.com/profit-gaurd
58. Nibble AI Negotiation — Shopify App Store, 2026 — https://apps.shopify.com/nibble-chat-bot
59. Nibble — BigCommerce Apps, 2026 — https://bigcommerce.com/apps/nibble-ai-negotiation
60. Negotiating chatbot Nibble — Fortune, 2024-07-16 — https://www.fortune.com/2024/07/16/negotiating-chatbot-nibble-ai-ecommerce
61. BargainIt — Shopify App Store, 2026 — https://apps.shopify.com/bargainit
62. How much do electronic shelf labels cost — KORONA POS, 2026-09-17 — https://koronapos.com/blog/how-much-do-electronic-shelf-labels-cost/
63. Nebraska Furniture Mart and Pricer SmartTAG — Pricer, 2014-02-05 — https://pricer.com/blog/nebraska-furniture-mart
64. Möbel Heinrich pilots VusionGroup ESLs — Retail Optimiser, 2025-03-12 — https://retail-optimiser.de/en/?p=21251
65. shopkeeper issue #45, owner discount approval (hobby project) — GitHub, 2025 — https://github.com/humberto0/shopkeeper/issues/45
