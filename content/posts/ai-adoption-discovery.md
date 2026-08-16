---
title: "AI Adoption, Before the AI"
subtitle: "Requirement discovery for a manufacturer's quote-to-drawing workflow"
period: "Jul 2026 – Aug 2026"
status: "Discovery phase complete"
impact: "Process maps · working prototype · role-based manuals"
date: 2026-08-08
kind: "Internship"
hook: "The client asked for AI. I started by drawing how they work today."
weight: 5

overview: "Two months inside an AI adoption project for a mid-sized manufacturer — where I learned that the model is never the bottleneck. The people who must change how they work have the least slack to learn."

highlight: "Product Manager Intern — AI adoption at a mid-sized manufacturer. Ran the discovery phase: role-by-role interviews, current-state process mapping, a working prototype, and rollout groundwork."

role:
  - title: "Requirement Discovery"
    module: "Interviewed working staff role by role; converged scattered asks into a concrete scope."
  - title: "Process Mapping"
    module: "Mapped the as-is quote-to-drawing workflow before any AI design was discussed."
  - title: "Prototype & Feedback"
    module: "Built a working prototype with AI assistance so frontline staff could walk the whole flow and react to it."
  - title: "Rollout Groundwork"
    module: "Wrote role-specific operation manuals and ran permission tests ahead of deployment."

challenge_points:
  - "The users are working sales staff — zero slack to learn a new tool mid-quarter."
  - "The owner's goals and the floor's daily reality described two different companies."
  - "Decisions made verbally drifted between meetings."

solution_points:
  - "Interviewed role by role, then drew the current state before proposing any future state."
  - "Wrote back after every meeting to lock scope and decisions on paper."
  - "One manual per role, not one manual per system."

decisions:
  - title: "Draw the current state before proposing AI"
    body: "The client asked for AI; I started with a diagram of how work flows today, confirmed line by line with the people doing it. An AI proposal built on a wrong map fails at rollout, quietly and expensively."
    tradeoff: "Weeks where nothing visibly 'AI' happened — which takes explaining. Slower to demo, faster to adopt."
  - title: "Write back after every meeting"
    body: "Verbal alignment decays. After each discussion I sent a short written summary — what was decided, what's in scope, what I'd do next — and invited corrections."
    tradeoff: "It can read as bureaucratic. But it converts memory into record, and record is what survives a disagreement."
  - title: "Fake the AI, validate the real flow"
    body: "The question to answer was whether the workflow held up, not whether the model was accurate. So I built a working prototype with a parametric mock standing in for generation, and let frontline staff walk it end to end: enter the requirement, see the draft, revise it in one sentence, sign off. The real model was left as a single swap point behind the same interface."
    tradeoff: "The output wasn't really AI-generated, which had to be said plainly in every demo — and it invited the question of whether this counted as finished. What it bought was workflow-level feedback: which step was missing, where people got stuck. A real API wouldn't have surfaced any of that."

architecture_title: "Discovery Workflow"
flow:
  - title: "Interview"
    detail: "Role by role, on the floor"
  - title: "Map"
    detail: "As-is process, confirmed line by line"
  - title: "Prototype"
    detail: "A working version of the whole flow"
  - title: "Feedback"
    detail: "Frontline walkthroughs, fix the gaps"
  - title: "Prepare"
    detail: "Role-based manuals, permission tests"

content_title: "What I Took From It"
---

> Client name and system details are confidential and deliberately not described here.

### The Reusable Part

What these two months left behind isn't a deck — it's a set of methods I'll keep using:

- **Interview guide** — interview role by role, starting from "walk me through what you actually did yesterday," never from "what features do you want."
- **Current-state map** — mark inputs, outputs, and sticking points for every step; nothing counts until the person who does the work has confirmed it line by line. Anything unverified stays a dashed line.
- **Write-backs** — a fixed three-part note after every meeting: what was decided, what's in scope, what I do next. Sent in writing, corrections invited.
- **Prototype first** — get a version people can actually operate end to end; the AI part can be mocked. What's being tested is the flow, not the precision.
- **Role-based manuals** — each covers only that role's own path; one page completes one task.
- **Permission tests** — walk each role's daily actions on their own account before launch, logging two kinds of findings: *can but shouldn't*, and *should but can't*.

### Reflection

The clearest thing I took from these two months: **AI adoption fails at the workflow, not the model.** Everyone in the building agreed the technology was impressive. What decided adoption was whether the person doing quotes at 4pm on a Tuesday could fit it into how they already work.

Which is the same lesson my dessert brand taught me from the other side — the people living inside a broken process have the least slack to change it. This time my job was to be the outside person who brings the slack: to watch, draw, confirm, and only then propose.
