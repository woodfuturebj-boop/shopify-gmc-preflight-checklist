# Shopify GMC Pre-Review Storefront Consistency Checklist (US/USD)

A practical, read-only self-audit checklist for Shopify merchants preparing for a **Google Merchant Center (GMC)** initial review or **Misrepresentation** appeal in the US/USD market.

> **Free Online Read-Only Self-Checker:** You can run an automated cross-page consistency check (no Shopify or GMC OAuth required, up to 2 verified verbatim conflicts shown free) at **[https://storepolicycheck.com](https://storepolicycheck.com)**.

---

## Why Storefront Contradictions Trigger GMC Misrepresentation Flags

Google's automated and manual reviewers cross-check what a shopper sees on your homepage, product page, footer policies, structured data (`JSON-LD`), and Merchant Center settings. Even legitimate stores often fail review because an announcement bar or theme update left outdated numbers in a policy page.

Use this checklist **before** clicking **"Request Review"** in Google Merchant Center.

---

## 1. Shipping Threshold & Policy Consistency
- [ ] **Announcement bar vs. Shipping Policy:** If your homepage header or product page says *"Free US shipping over $50"*, verify `/policies/shipping-policy` (and any FAQ/help page) does not still say *"Free shipping over $69"* or another outdated number.
- [ ] **Shipping Policy reachable:** Confirm your footer Shipping Policy link returns `200 OK` (no broken `404` links) and clearly states handling time + transit time or *"Calculated at checkout"*.
- [ ] **GMC Shipping Settings match live site:** Ensure the free-shipping threshold configured inside GMC matches your public US/USD storefront.

## 2. Return Window, Return Shipping Fees & Restocking Fees
- [ ] **Return window consistency:** Check that your homepage, product page tabs, FAQ, and `/policies/refund-policy` all state the same general return window (e.g., *30 days* everywhere—not *14 days* in one place and *30 days* in another).
- [ ] **Two-stage deadlines clearly explained:** If you allow 30 days to request a return and 14 days to ship it back after approval, state both stages clearly so reviewers do not read them as conflicting timelines.
- [ ] **Return shipping & restocking fees:** Never advertise unconditional *"Free Returns"* in a banner or product tab while your Refund Policy charges return shipping labels or a restocking fee for change-of-mind returns. Clearly separate defective/damaged returns from change-of-mind returns.

## 3. Product Variant Price, Currency & JSON-LD Markup
- [ ] **US/USD currency alignment:** When accessed from a US IP, ensure both the visible primary buy-box price and the page's `application/ld+json` `Offer.priceCurrency` are `USD`.
- [ ] **Variant-level price accuracy:** For multi-variant products (`/products/handle?variant=...`), confirm the selected variant's live selling price (excluding strikethrough `compare-at` prices) matches both the variant JSON-LD `Offer.price` and your GMC product feed price.

## 4. Contact Info, Domain Consistency & Crawlability
- [ ] **Working contact entry:** Provide a reachable Contact page with a working contact form, valid business email (`support@yourdomain.com`), and clear response expectations.
- [ ] **Clean template copy:** Remove leftover placeholder text (`[Insert Address]`, `[Company Name]`, or another store's brand/email copied from a template).
- [ ] **`robots.txt` check:** Keep default Shopify `/admin` and `/checkouts` blocks intact, and confirm you have not accidentally disallowed `/products/` or `/policies/` for `Googlebot`, `Storebot-Google`, or `Googlebot-Image`.
- [ ] **Fulfillment transparency (if cross-border):** If your business registration address and warehouse shipping origin are in different regions, briefly state both clearly in your Shipping/About page so expectations are transparent.

---

## Independent Boundary Note

Checking public storefront consistency catches public HTML, policy, and pricing contradictions before an appeal. However, GMC reviews also evaluate private account-level factors (business identity verification, payment methods, fulfillment history, and linked accounts) that no public page scanner can see.

Run a fast read-only public check here: **[https://storepolicycheck.com](https://storepolicycheck.com)**

---

## 中文速查要点（独立站 GMC 复审前 6 项硬核自查）
1. **免邮门槛一致**：顶栏/商品页写的美国免邮金额（如满 \$50），必须与页脚 Shipping Policy 和 GMC 后台完全一致；
2. **退货天数一致**：商品页、FAQ 与 Refund Policy 的无理由退货天数不可打架；
3. **退货运费透明**：顶栏写无条件 Free Returns，政策页就不能写“买家自付退货运费”或扣入库费（质量问题与个人原因需分开写清）；
4. **变体现价与代码一致**：带 `?variant=` 的商品页非划线现价、底层 JSON-LD `Offer.price`（USD）和 GMC Feed 报价必须完全一致；
5. **联系方式与模板清理**：确保联系页面和政策页无 `404`、无残留别人店名/异域客服邮箱或未替换的 `[占位符]`；
6. **`robots.txt` 放行**：确认未误拦截 `Googlebot`、`Storebot-Google` 或 `Googlebot-Image` 抓取 `/products/` 与 `/policies/`。

在线只读核对工具（免绑后台，免费看前 2 条逐字冲突证据）：**[https://storepolicycheck.com](https://storepolicycheck.com)**
