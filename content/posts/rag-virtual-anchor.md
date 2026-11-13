---
title: "Virtual Anchor Generation System"
subtitle: "A RAG system that turns a stock ticker into a financial news video"
period: "Feb 2025 – Dec 2025"
date: 2025-12-31
kind: "Capstone · Published"
hook: "I led a four-person team from system architecture to a published paper."
weight: 10
featured: true
card_art: "benchmark"
claim: "I picked the model by testing under real constraints, and led a four-person team."
proof: "10 models benchmarked · bge-m3 79.59% · TCSE 2025"

context: "Capstone project, February to December 2025. Our four-person team built a system that turns a stock ticker into a finished news broadcast video."
role: "Team lead. I owned the RAG retrieval framework and the Flask backend, and integrated four members' modules: news collection, script generation, voice, and video rendering."
did: "I built a financial Q/A test set, benchmarked 10 embedding models on it, and added a normalization layer for financial terms."
result: "bge-m3 scored a 79.59% hit rate and 65.54% MRR. With RAG, verifiable facts in the scripts rose by 80%. We placed 7th of 80 teams and published at TCSE 2025."
reflection: "In school I thought the model mattered most. At work I found that the framework, the tools, and the context matter more."

image: "/images/rag-benchmark-en.svg"
image_caption: "My benchmark of 10 embedding models on a self-built financial Q/A set. BAAI/bge-m3 scored highest on both hit rate and MRR, so we used it."

demo_link: "https://github.com/ollie33/Virtual-Anchor-Generation-System"
demo_label: "Source Code"
---

The first embedding model we tried worked badly, and that is when I started studying embedding models. We had three constraints. The content was in Chinese, the domain was finance, and our budget was limited, so we could only use general open-source models.

So I built a financial Q/A test set of our own and compared 10 embedding models on it. BAAI/bge-m3 scored highest, with a 79.59% hit rate and 65.54% MRR. I also added a normalization layer for financial terms, so a phrase in the news can match the technical indicator behind it. After RAG went in, verifiable facts in our scripts rose by 80%.

A full video takes about 10 to 15 minutes to generate. Our professor suggested generating it in segments, and the team discussed it and agreed. I implemented the SSE streaming, so users see a progress signal within 5 seconds and can start watching the first segment after about 3 minutes.
