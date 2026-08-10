# Flowline

**A personal productivity dashboard that drives your next action automatically.**

Flowline eliminates the daily decision of "what should I work on right now?" by ranking your task queue against three factors: deadline urgency, priority weight, and whether the task actually fits your next open time block. The result is a single, confident recommendation — with a plain-language reason — updated every time your situation changes.

[**Live Demo →**](https://integratorjeffj.github.io/flowline)

---

## What it does

The **Next Up** card always shows one task: the highest-scoring item that fits your current available time. It explains its own reasoning in plain English — no black box, no mystery.

Behind that card, a weighted scoring formula runs across your full task list:

```
score = priority weight + urgency (deadline proximity) + effort-fit bonus
```

- **Priority weight** — High (30), Medium (18), Low (8)
- **Urgency** — Overdue (40), Due today (25), This week (8), Next week (1)
- **Effort-fit bonus** — +10 if the task fits your open block, +3 if it's close

The task that scores highest and fits the time you actually have wins. Every time you complete, snooze, or add a task, the recommendation updates instantly.

---

## Features

- **Next Up card** — single recommended action with plain-language reasoning
- **Day River timeline** — visual map of your day: focus blocks, meetings, and breaks, with a live "now" marker
- **Weighted task ranking** — deadline + priority + effort fit, recalculated on every change
- **Interactive task list** — check off tasks, drag to reorder, use arrow controls
- **Add task form** — no code required, add name, priority, effort estimate, and due date
- **KPI strip** — completed today, overdue count, focus streak, open focus time
- **Weekly load bar chart** — pure CSS, no charting library
- **Focus allocation donut** — conic-gradient, no charting library
- **Dark mode** — full CSS-variable theme system, preference persisted in localStorage
- **Zero dependencies** — no frameworks, no CDN calls, no build step. One HTML file.

---

## Why it's built this way

Most productivity tools show you everything and let you decide. Flowline makes the decision for you, then shows its work. The ranking logic is intentionally transparent so the recommendation feels trustworthy rather than arbitrary.

The no-dependency, single-file architecture means it loads instantly in any environment: a locked-down browser, an email attachment viewer, a sandboxed preview. Every value renders directly in the HTML — nothing depends on JavaScript executing to show you a number.

---

## Running it locally

No install required.

```bash
git clone https://github.com/integratorjeffj/flowline.git
cd flowline
open index.html
```

Or just visit the [live demo](https://integratorjeffj.github.io/flowline).

---

## Roadmap

- [ ] Config layer — JSON-driven widget layout so users can customize without touching code
- [ ] Calendar integration — pull real time blocks from Google Calendar or M365
- [ ] Task source connectors — import from Todoist, Asana, or a simple CSV
- [ ] AI-powered task intake — describe work in plain language, Flowline extracts priority, effort, and deadline
- [ ] Team view — manager-facing summary of team focus allocation

---

## Also built

**AI Proposal Workflow**
Designed an AI-assisted proposal workflow that turns technical and commercial requirements into structured recommendations, pricing, labor, and engineering guidance with explicit human review. In one five-day period, the workflow supported nine proposals representing more than $400K in quoted work.

**Guided Network Deployment Tools**
Built guided technical workflows for complex network configuration tasks, including WireGuard deployment and RouterOS configuration. The tools combine structured inputs, validation, generated configuration, and readback checks so less-experienced technicians can execute advanced work more consistently and with fewer errors.

**ProcessForge**
Developing an AI-native operations platform designed to connect company knowledge, workflows, approvals, automation, and business systems into a governed operating layer. The architecture uses Git-aware development, human approval gates, manifest-driven validation, drift detection, and explicit controls around AI-initiated changes.

**AI Employee Enablement Framework**
Created a coaching-led framework for moving employees from AI experimentation to independent, repeatable performance. The model combines guided practice, workflow analysis, reusable prompts and SOPs, capability assessment, and a process for converting successful AI-assisted work into reusable organizational knowledge.

---

## About

Built by [Jeff Jenkins](https://github.com/integratorjeffj) — AI integration, automation, and managed technology operations.

Currently focused on AI adoption and enablement roles: helping organizations move from AI experimentation to repeatable, governed, business-value-producing workflows.
