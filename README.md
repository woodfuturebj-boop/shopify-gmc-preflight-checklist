# Google Merchant Center Shopify Pre-Appeal Checklist 2026 (5-Phase Cooldown Guard)

Complete all **5 phases** below before clicking **Request Review** in Google Merchant Center to avoid wasting a 7-day appeal cooldown.

Interactive web checklist & free zero-login diagnostic tools: **[https://storepolicycheck.com/tools/gmc-appeal-readiness-checklist](https://storepolicycheck.com/tools/gmc-appeal-readiness-checklist)**

---

## Phase 1: Business Identity, Street Address & Support Email MX
- [ ] Identical physical street address across `/pages/contact`, Footer, Terms of Service, and Privacy Policy
- [ ] Custom-domain support email publishes valid DNS MX records (emails do not bounce) -> [Free MX & Entity Checker](https://storepolicycheck.com/tools/shopify-trust-email-address-checker)
- [ ] Zero leftover template emails, `Lorem ipsum` placeholders, or HTTP 404 footer links
- [ ] Honest corporate registration vs. 3PL warehouse fulfillment disclosure

## Phase 2: Shipping & Return Policy Verbatim Cross-Page Parity
- [ ] Homepage announcement bar free-shipping threshold matches `/policies/shipping-policy` to the exact dollar
- [ ] Handling days (e.g. `1–2 business days`) and transit days stated explicitly
- [ ] `/policies/refund-policy` states exact return window (`14+ days` statutory minimum for UK/EU)
- [ ] Explicit clause stating **who pays return shipping postage** and any restocking fee -> [Free 22-Rule Verbatim Audit](https://storepolicycheck.com)

## Phase 3: `?variant=` JSON-LD Price, Dawn Schema & Bundle/Subscription App Overrides
- [ ] Every `?variant=` visible buy-box price equals `Offer.price` in `application/ld+json` -> [Free Variant JSON-LD & Plugin Checker](https://storepolicycheck.com/tools/shopify-variant-json-ld-price-checker)
- [ ] Kaching Bundles / WideBundle defaults to the **1-unit single pack** on initial page load
- [ ] Recharge / Seal / Appstle defaults to **One-Time Purchase** (not Subscribe & Save)
- [ ] Shopify Dawn `{{ product | structured_data }}` checked for conflicting SEO app `hasMerchantReturnPolicy` days -> [Dawn Copy-Paste Liquid Patch](https://storepolicycheck.com/guides/shopify-dawn-missing-hasmerchantreturnpolicy-gmc-impact)
- [ ] Adding 1 item to `/cart.js` injects zero auto-checked paid shipping protection

## Phase 4: Jan 31, 2027 `500×500 px` Product Images & `robots.txt` Crawl Access
- [ ] All primary (`image_link`) and gallery (`additional_image_link`) photos measure **≥ 500 × 500 px** (mandatory Jan 31, 2027) -> [Free 5,000-SKU 500×500 Image Checker + CSV Export](https://storepolicycheck.com/tools/gmc-image-size-checker)
- [ ] Zero promotional text (`FREE SHIPPING`, `50% OFF`) in product titles or `0g` physical weights
- [ ] `robots.txt` permits `Googlebot`, `Googlebot-Image`, and `Storebot-Google` -> [Free robots.txt Tester](https://storepolicycheck.com/tools/shopify-robots-txt-googlebot-tester)

## Phase 5: Private GMC Backend Sync (Owner Manual Verification)
- [ ] GMC **Business Information** legal name, street address, and verified phone match storefront footer
- [ ] GMC **Shipping & Returns** settings match storefront thresholds, handling/transit days, and return fees
- [ ] Google & YouTube feed synced with zero disapproved price/availability items
- [ ] Real Incognito guest checkout tested: shipping & tax match policy with zero surprise fees

---

## Read-Only MCP Server & 2026 Tool Comparison (No Monthly Subscription)
- **Read-Only MCP Server for Claude / Cursor (0 Credentials)**: [github.com/woodfuturebj-boop/storepolicycheck-mcp](https://github.com/woodfuturebj-boop/storepolicycheck-mcp) · [storepolicycheck.com/mcp](https://storepolicycheck.com/mcp)
- **9-Tool Public Pricing Matrix ($29 One-Time Pass vs. $28–$149/mo Subscriptions)**: [storepolicycheck.com/compare/shopify-gmc-audit-tools](https://storepolicycheck.com/compare/shopify-gmc-audit-tools)
