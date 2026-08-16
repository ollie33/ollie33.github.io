---
title: "Virtual Anchor Generation System"
subtitle: "Using RAG to move a financial video pipeline from fluent to factual"
period: "Feb 2025 – Dec 2025"
status: "Published — TCSE 2025"
impact: "Top 7 / 80 · +80% factual density"
date: 2025-12-31
kind: "Capstone · Published"
hook: "Technical depth: led an AI system from architecture to published paper."
weight: 10

overview: "Stock ticker in, finished broadcast video out in under 10 minutes — with retrieval grounding the script in what actually happened that day."

highlight: "Led a four-person team; owned the retrieval framework and backend architecture."

role:
  - title: "Project Leader"
    module: "Set goal and scope; integrated four members' modules and fixed the seams between them."
  - title: "RAG Retrieval Framework"
    module: "News filtering, model selection, and a hand-built semantic database for financial terms."
  - title: "Backend Architecture"
    module: "Flask control hub, job management, SSE streaming."

challenge_points:
  - "Markets move daily; a professional video takes hours to make."
  - "Without retrieval, the LLM wrote fluently and said nothing — zero verifiable facts."
  - "Generic embeddings can't link 'death cross' in news to the indicator that produced it."

solution_points:
  - "Benchmarked 5 embedding models on a self-built financial Q/A set."
  - "Hand-built a semantic layer aligning news language with technical indicators."
  - "SSE streaming: first progress signal within 5 seconds."

decisions:
  - title: "Choose the embedding model with a benchmark, not a hunch"
    body: "No benchmark existed for Chinese financial retrieval, so I built a Q/A set and compared five models. BAAI/bge-m3 won — 73.59% hit rate, 65.54% MRR."
    tradeoff: "The eval set cost time we could have spent on features, but without it every later quality drop would be unattributable."
  - title: "Add a semantic standardisation layer"
    body: "Even the best model couldn't match news phrases to indicator values — they don't align in vector space. I hand-built a database normalising both into one shared vocabulary."
    tradeoff: "Hand-built means it doesn't scale to new domains. Right for a semester project; would need to be self-extending to productise."
  - title: "Switch to SSE — a UX decision, not a technical one"
    body: "Long generation jobs meant users stared at a blank screen — where they leave. SSE streams progress back within 5 seconds."
    tradeoff: "Total generation time didn't drop one second. Only perceived performance changed — which turned out to be the one that mattered."

architecture_title: "System Architecture"
flow:
  - title: "Scrape"
    detail: "MoneyDJ / Anue / Yahoo Finance + yfinance"
  - title: "Standardise"
    detail: "News language ↔ technical indicators"
  - title: "Retrieve"
    detail: "bge-m3 + FAISS"
  - title: "Generate"
    detail: "Indicators + top-5 passages → OpenAI"
  - title: "Speak"
    detail: "Google Cloud TTS"
  - title: "Render"
    detail: "Unity + Live2D, pushed over SSE"

image: "/images/rag-architecture.jpg"
image_caption: "Five layers, 11 pipeline steps, no human in the loop."

demo_link: "https://github.com/ollie33/Virtual-Anchor-Generation-System"

content_title: "Results & Reflection"
---

### Results

- **+80% factual density** — counted verifiable facts across paired scripts, with and without RAG, on the same tickers.
- **Hours → under 10 minutes**, fully automated.
- **Top 7 of 80**, FCU CS Capstone Competition · **full paper published** at TCSE 2025.

### Reflection

If I rebuilt it, I'd rebuild it **as agents**. Our pipeline treats every story the same way — but an earnings call, a sudden shock, and a quiet consolidation need different retrieval and different narrative shapes.

An agent architecture would let the system decide what to look for and how to tell it. That's this project's clearest ceiling — and I only saw it after finishing.
