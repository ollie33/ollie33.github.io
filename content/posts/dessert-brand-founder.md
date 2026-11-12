---
title: "Seayou — A Dessert Brand from Zero"
subtitle: "Owning a whole value chain alone: recipe, costing, pricing, marketing, customers"
period: "Aug 2023 – Dec 2024"
date: 2024-12-31
kind: "Founder"
hook: "Business ownership: pricing, customers, and a whole value chain alone."
weight: 40
claim: "I ran the whole value chain alone, and found improvements in the daily repeated work."

context: "A handmade dessert brand I built from zero and ran alone for seventeen months, from August 2023 to December 2024. The brand ended in late 2024."
role: "Founder and sole operator. Recipes, costing, pricing, marketing, orders, and delivery were all mine."
did: "I ran four product lines, lemon tarts, soft cookies, biscuits, and cakes, selling through Instagram and in-person markets. After the brand ended, I built an n8n flow to automate the order admin."
result: "About 500 online orders and NT$10,000–30,000 in monthly revenue. The automation test showed my two hours of daily order work could become about fifteen minutes of review."
reflection: "I put up with that admin burden the whole time the shop ran, and only had room to fix it after it ended. Since then, when I look at any workflow, I start from the task someone repeats every day."

image: "/images/seayou-n8n.png"
image_caption: "The n8n flow, validated on historical order emails. Gmail trigger, AI extraction, a JavaScript validation step, and clean rows appended to Google Sheets."
image2: "/images/seayou-market.jpg"
image2_caption: "The market stall, with all four product lines."

demo_link: "https://www.instagram.com/seayou_dessert/"
demo_label: "Instagram"
---

Order emails came in inconsistent formats. Every day I spent about two hours retyping them into my records by hand. While the shop was running, I never had the time to fix this.

After the brand ended, I taught myself n8n and rebuilt the order admin process. A Gmail trigger picks up order emails, Gemini and GPT extract the structured data, a JavaScript validation node reshapes it into a fixed schema, and the clean rows go into Google Sheets. I chose n8n over pure no-code tools because AI-extracted data does not reliably match the destination schema, and I needed that custom validation step after the AI.

I validated the flow on historical order emails only. It never ran in live operations. The test showed that about two hours of daily order admin would have become about fifteen minutes of review.
