---
title: "AI Adoption, Before the AI"
subtitle: "Requirement discovery for a manufacturer's quote-to-drawing workflow"
period: "Jul 2026 – Aug 2026"
status: "Discovery phase complete"
impact: "Process maps · role-based manuals · permission tests"
date: 2026-08-08
kind: "Internship"
hook: "The client asked for AI. I started by drawing how they work today."
weight: 5

overview: "Two months inside an AI adoption project for a mid-sized manufacturer — where I learned that the model is never the bottleneck. The people who must change how they work have the least slack to learn."

highlight: "Ran the discovery phase: role-by-role interviews, current-state process mapping, manuals, and permission testing."

role:
  - title: "Requirement Discovery"
    module: "Interviewed working staff role by role; converged scattered asks into a concrete scope."
  - title: "Process Mapping"
    module: "Mapped the as-is quote-to-drawing workflow before any AI design was discussed."
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
  - title: "One manual per role, not per system"
    body: "A manager, a salesperson, and a drafter touch the same system in completely different ways. I wrote each of them their own manual covering only their path."
    tradeoff: "Three documents to keep in sync instead of one. Adoption happens per person, though — not per feature list."

architecture_title: "Discovery Workflow"
flow:
  - title: "Interview"
    detail: "Role by role, on the floor"
  - title: "Map"
    detail: "As-is process, confirmed line by line"
  - title: "Write back"
    detail: "Lock scope and decisions on paper"
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
- **Role-based manuals** — each covers only that role's own path; one page completes one task.
- **Permission tests** — walk each role's daily actions on their own account before launch, logging two kinds of findings: *can but shouldn't*, and *should but can't*.

### Reflection

The clearest thing I took from these two months: **AI adoption fails at the workflow, not the model.** Everyone in the building agreed the technology was impressive. What decided adoption was whether the person doing quotes at 4pm on a Tuesday could fit it into how they already work.

Which is the same lesson my dessert brand taught me from the other side — the people living inside a broken process have the least slack to change it. This time my job was to be the outside person who brings the slack: to watch, draw, confirm, and only then propose.
