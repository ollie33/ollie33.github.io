---
title: "AI Customer Service Testing at e-Insure"
subtitle: "Splitting the problems into prompt, dataset, and engineering layers"
period: "Sep 2026 – Present"
date: 2026-09-01
kind: "Internship"
hook: "I took over testing an AI customer service and sorted its problems into three layers."
weight: 15
featured: true
card_art: "layers"
claim: "I split an AI customer service's problems into three layers, and the changes I proposed clearly raised accuracy in retesting."
proof: "AI product testing · Root-cause analysis · RAG optimization"

context: "e-Insure, from September 2026. An AI customer service was almost finished but stuck, because the two-person support team had no time to test it."
role: "Digital Product Manager Intern. I design and run the tests; engineers own the RAG framework and the fixes."
did: "I took over the testing, sorted the feedback into prompt, dataset, and engineering issues, and compared 3 models myself."
result: "The current model and one other model performed equally well, and the third was clearly worse, so we kept the current model and adjusted the RAG framework instead. After the changes, retesting with the same questions showed clear accuracy gains for both FAQ questions and likely user questions. The bot has not launched yet and is in its final round of testing."
reflection: "Sorting each problem into a layer told the engineers where to make the fix. I learned that the most useful thing I can do is find where the problem is and bring evidence. The engineers own the fix."

image: "/images/einsure-layers.svg"
image_caption: "How I sort the support team's feedback. Each problem goes to the layer that needs the fix, and engineers make the change."
---

The AI customer service was nearly done when I joined, but it had not launched. The customer service team has only two people, and they were too busy to test it. I offered to take over the testing. I tested the bot myself and organized the results so the team only needed to give short feedback.

When the feedback came back, I analyzed each problem and sorted it into three groups: prompt, dataset, or engineering. Testing the models was one part of this analysis, and I ran it at the same time with a separate set of questions.

I compared 3 models. The current model and one other performed equally well, and the third was clearly worse. The current model was good enough, so instead of switching models, I proposed changes to how the RAG framework prepares and retrieves its data. I made these decisions first, and then asked the engineers to make the changes. After the changes, the bot was retested with the same questions. Accuracy rose clearly on both questions covered by the FAQ and questions users are likely to ask. The bot has not launched yet and is in its final round of testing.
