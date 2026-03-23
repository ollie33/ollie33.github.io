---
title: "RAG-Based Virtual Anchor Generation System"
subtitle: "基於 RAG 技術之虛擬主播生成系統"
status: "Completed (Top 7/80)"
impact: "+80% Content Quality"
overview: "An end-to-end automated video generation framework integrating RAG retrieval with real-time news data analysis, streamlining professional video production from several hours to under 10 minutes."
period: "Fab 2025 – Dec 2025"

role:
  - title: "Project Leader & System Architect"
    module: "Designed the End-to-End architecture integrating LLMs, Vector DBs, and front-end rendering."
  - title: "AI/Prompt Engineer"
    module: "Optimized retrieval strategies and prompt engineering to significantly reduce AI hallucinations."
  - title: "Backend Developer"
    module: "Implemented Flask backend and Server-Sent Events (SSE) for low-latency streaming."

learnings:
  - title: "Data Quality Outperforms Model Size"
    description: "Integrating a well-structured RAG framework with FAISS provided a much more significant boost to response accuracy than merely upgrading the underlying LLM."
  - title: "Systematic Prompts Ensure Stability"
    description: "Designing semantic standardization in prompts was crucial for seamlessly triggering the correct facial expressions on the Unity/Live2D frontend."
  - title: "Latency is the Ultimate UX Killer"
    description: "Transitioning from traditional request-response to SSE streaming taught me the critical importance of optimizing Time to First Token (TTFT) for real-time applications."

challenge_points:
  - "Severe LLM hallucinations caused inaccurate financial news reporting."
  - "High latency in traditional generation loops disrupted the real-time broadcasting rhythm."
  - "Unstructured AI text output failed to consistently trigger frontend animation controls."

solution_points:
  - "Self-taught and integrated a RAG framework (LangChain + FAISS) within one week."
  - "Implemented Flask + SSE for real-time, low-latency text-to-speech data streaming."
  - "Engineered semantic standardization to ensure perfect lip-sync and expression triggering on Unity/Live2D."

image: "/images/rag-architecture.jpg"
demo_link: "https://github.com/your-username/your-repo-link"
---

