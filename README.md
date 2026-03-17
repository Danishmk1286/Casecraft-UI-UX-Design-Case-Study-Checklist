# Casecraft

**A step-by-step checklist for UI/UX students building their first portfolio case study.**

Casecraft guides you through every stage of a case study — from writing a problem statement to publishing your work — broken down into 18 deliverables and ~96 individual tasks. Each task includes a practical tip explaining *why* it matters, not just *what* to do.

It runs entirely in the browser. No login. No setup. Open the file and start working.

---

## Why this exists

Most beginner UI/UX resources are either too abstract (phases and principles with no concrete output) or too prescriptive (fill in this exact template). Casecraft sits in the middle.

It's organised by **deliverable**, not by phase. You always know what you're building next — a Research Document, a Persona, a Prototype — not just what "stage" you're in. That distinction matters when you're new and the process feels formless.

Three failure points it directly addresses:

- **Skipping research** — because they don't know what research should produce. The Research Document deliverable makes the output concrete.
- **Jumping to high-fidelity too early** — because wireframes feel like "not real design." Seven deliverables come before high-fidelity screens, making that clear.
- **Never documenting the process** — because students focus on the final product. Documentation, Visual Storytelling, and Case Study Write-Up are treated as real work, not afterthoughts.

---

## What's inside

### 18 deliverables, ~96 tasks

| # | Deliverable | Tasks |
|---|---|---|
| 1 | Project Brief | 5 |
| 2 | Research Plan & Execution | 6 |
| 3 | Competitive Analysis | 4 |
| 4 | Research Synthesis | 3 |
| 5 | User Persona | 6 |
| 6 | Problem Statement & Scope | 5 |
| 7 | Information Architecture & User Flows | 4 |
| 8 | User Journey Map | 6 |
| 9 | Ideation & Concept Exploration | 6 |
| 10 | Wireframes | 7 |
| 11 | Style Guide / Mini Design System | 6 |
| 12 | High-Fidelity UI Screens | 6 |
| 13 | Prototype | 5 |
| 14 | Usability Test Report | 5 |
| 15 | Final Design & Developer Handoff | 5 |
| 16 | Documentation & Artifact Archive | 3 |
| 17 | Case Study Write-Up | 8 |
| 18 | Review, Polish & Publish | 6 |

Each task has an inline tip — plain language, practical, aimed at someone doing this for the first time.

---

## Features

**Two views**

- **Quick ref** — a card grid showing all 18 deliverables with per-card progress bars. Good for getting an at-a-glance sense of where you are.
- **Full guide** — the complete task list, expandable per deliverable. Click any Quick ref card to jump directly to that deliverable in Full guide.

**Progress tracking**

- Overall progress bar and percentage in the sidebar
- Per-deliverable task counts in the nav and on each card
- Deliverables turn green when every task is complete

**Sidebar navigation**

- Jump to any deliverable directly
- Visual indicators for completed (green) and active (orange) deliverables
- Click an active item to collapse it

**Confetti** — fires when you complete a deliverable. Small thing, matters.

**Scalability footer** — a closing card explaining how to adapt the skeleton to other project types (product redesign, mobile app, design system, service design).

---

## How to use it

**Option 1 — Open directly**

Download `casecraft.html` and open it in any browser. No server needed.

**Option 2 — Host it**

Drop `casecraft.html` into any static hosting service (GitHub Pages, Netlify, Vercel). No build step, no dependencies.

**Option 3 — Fork and customise**

The deliverable data lives in a single `D` array near the top of the `<script>` block. Each deliverable follows this structure:

```js
{
  id: "brief",
  title: "Project Brief",
  why: "One sentence explaining why this deliverable matters.",
  tasks: [
    { l: "Task label", t: "Tip text explaining how to approach it." },
    ...
  ]
}
```

To add a deliverable: append an object to the array.  
To remove one: delete it from the array.  
To adapt for a different project type: swap out tasks while keeping the structure.

---

## Design decisions

**Deliverables over phases.** The double-diamond and similar phase models are useful mental models, but they're hard to act on. "What am I producing right now?" is a more useful question than "what phase am I in?" Casecraft answers the first question.

**One inline tip per task.** Not a tooltip, not a separate page, not a hover state. The tip is always visible, right below the task. Beginners read the task and immediately want to know "but how?" — the tip answers before they have to ask.

**Tips hide when a task is checked.** Once you've done something, the instruction is noise. Hiding completed tips keeps the list scannable.

**Sequential ordering is deliberate.** Each deliverable feeds the next. The Project Brief informs Research. Research informs the Persona. The Persona informs the Problem Statement. Breaking this sequence is the most common cause of a weak case study.

**No login, no backend, no tracking.** Progress lives in the session. Refreshing resets it. This is intentional for a v1 — the goal is zero friction to open and start.

---

## Adapting for other project types

The skeleton generalises:

```
Problem → Research → Define → IA → Ideation → Design → Test → Handoff → Document → Publish
```

Swap domain-specific deliverables for equivalents:

| Case study | Other project types |
|---|---|
| User persona | Stakeholder map |
| User journey map | Service blueprint |
| Wireframes | Content wireframes / paper prototypes |
| Usability test report | Stakeholder feedback log |
| Case study write-up | Project retrospective / post-mortem |

---

## Who this is for

- **Students** building their first or second portfolio piece
- **Career switchers** doing self-initiated UI/UX projects
- **Bootcamp graduates** who want a structured process reference
- **Junior designers** at companies looking for a lightweight process guide

It is intentionally scoped to a single case study, not a full design process framework. It does one thing and tries to do it well.

---

## Contributing

Issues and pull requests are welcome. If you spot a task that's missing, a tip that's wrong, or a deliverable that doesn't belong — open an issue.

If you're adapting Casecraft for a specific project type (e.g. a design system checklist, a mobile app checklist), consider opening a PR with a new data file. The goal is a family of single-file checklists, each scoped and opinionated.

---

## Licence

MIT. Use it, fork it, adapt it, share it.

---

*Built for UI/UX students who want to know what to do next, not just how design works in theory.*
