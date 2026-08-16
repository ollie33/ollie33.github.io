---
title: "Seayou — A Dessert Brand from Zero"
subtitle: "Owning a whole value chain alone: recipe, costing, pricing, marketing, customers"
period: "Aug 2023 – Dec 2024"
status: "Closed by choice"
impact: "~500 online orders · NT$10–30k / month"
date: 2024-12-31
kind: "Founder"
hook: "Business ownership: pricing, customers, and knowing when to stop."
weight: 20

overview: "A handmade dessert brand I ran solo for seventeen months — and where I learned that the hard part of a bad process isn't noticing it, it's having the slack to fix it."

highlight: "Founder, sole operator — four product lines, sold through Instagram and in-person markets."

role:
  - title: "Founder & Sole Operator"
    module: "Product, costing, pricing, marketing, fulfilment, customers — all of it, alone."
  - title: "Automation (post-closure)"
    module: "Self-taught n8n; rebuilt the order-admin process and validated it on historical emails."

challenge_points:
  - "Every function of a business, alone, alongside full-time study."
  - "Order emails arrived in inconsistent formats — ~2 hours of manual retyping a day."
  - "By late 2024, coursework and an incoming internship made quality impossible to hold."

solution_points:
  - "Priced from ingredient cost up: NT$45 entry biscuit → NT$60 premium variants."
  - "Markets for face-to-face feedback; Instagram for repeat purchase."
  - "Closed while the product was still good, rather than let it decay."

decisions:
  - title: "Two channels, two different jobs"
    body: "Markets weren't for volume — they were the only place I could watch a customer's face at the first bite. That fed recipes and packaging. Instagram turned those people into repeat buyers."
    tradeoff: "A market day often earned less than the same hours filling orders. I booked it as research cost, not sales cost."
  - title: "A price ladder, not a flat price"
    body: "NT$45 plain biscuit made trying the brand a low-stakes decision; NT$60 variants and a two-tart bundle (NT$140) lifted the basket once someone said yes."
    tradeoff: "More SKUs means more prep and leftover risk for one person — I capped it at four lines."
  - title: "Close it rather than let it decay"
    body: "Handmade quality is bound to hours invested. Pushing through senior year would have meant slower shipping, worse product, and a reputation spent down by me."
    tradeoff: "I gave up a stable customer base. But a brand run badly was worth nothing to them or me."

architecture_title: "Order Automation (built after closing)"
flow:
  - title: "Gmail Trigger"
    detail: "Filter order notifications"
  - title: "AI Agent"
    detail: "Extract structured data from messy text"
  - title: "Code Node"
    detail: "Validate & reshape to schema"
  - title: "Sheets"
    detail: "Append clean rows"

image: "/images/seayou-market.jpg"
image_caption: "The market stall — four product lines, handwritten price tags."

demo_link: "https://www.instagram.com/seayou_dessert/"

content_title: "Results & Reflection"
---

> **On the automation:** built **after the brand closed**, as a self-teaching exercise. Validated on historical order emails — **never ran in live operations**. The estimate: my ~2 hours a day of order admin would have become ~15 minutes of review.

### Results

- **~500 online orders** over 17 months, plus in-person market sales.
- **NT$10–30k monthly revenue**, sustained alongside full-time study.
- **Why n8n over Zapier/Make:** AI-extracted data doesn't reliably match the destination schema — I needed a custom JS validation node after the AI step, which pure no-code tools can't do.

### Reflection

I tolerated that admin burden for over a year, and only had the slack to systematise it **after** I stopped. What separates noticing a pain point from fixing one is usually not skill — it's slack.

That's why, in requirement interviews, "what feels inconvenient?" rarely surfaces anything. What works is watching which motions someone repeats every single day.
