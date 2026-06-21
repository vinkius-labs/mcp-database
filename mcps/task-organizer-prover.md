# Task Organizer Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/task-organizer-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A team asked an AI to organize 28 tasks for a launch. The AI produced a flat list. No priorities. No dependencies. Everything 'estimated at 2-4 hours.' Capacity: 120 productive hours available, list totaled 210h. Launch week: 3 blocking dependencies discovered mid-sprint because nobody mapped them. Critical path was 40% longer than the timeline. This tool forces five axes: priority classification with Eisenhower matrix, dependency mapping with critical path, estimation rigor with PERT, capacity awareness with WIP limits, and outcome alignment with SMART deliverables.

## Description
## The Problem

AI agents produce task plans that look organized but collapse under real-world pressure. They fail on five axes:

- **Priority Blindness** — 'all tasks are important' means nothing is prioritized. A hospital has 12 improvement projects, all labeled 'Priority 1.' After 6 months: all 12 are 15-25% complete. None delivered value.
- **Dependency Ignorance** — flat lists hide blocking chains. 'Frame walls' appears before 'Pour foundation.' Dependencies discovered mid-sprint cause cascading delays.
- **Estimation Fantasy** — 'about 2 hours' without PERT, historical calibration, or complexity factors. Gut-feel estimates are off by 2-4x on average.
- **Capacity Amnesia** — 8 hours in a day ≠ 8 productive hours. Meetings, admin, and context switching (23 min per switch, UC Irvine) reduce real output to 4-5 hours.
- **Outcome Disconnect** — 'Write report' is an activity, not a deliverable. Without SMART criteria and acceptance conditions, tasks are never truly done.

### How It Works

Task Organizer Prover uses 5 Decision Pivots — boolean checkpoints that force the agent to validate its own task plan:

1. **prioritized** — Eisenhower matrix applied, forced ranking, ICE scoring, cost of delay quantified?
2. **dependenciesMapped** — Blocking chains identified, critical path determined, parallel opportunities found?
3. **estimatesRigorous** — Three-point estimates with PERT formula, historical calibration, buffer added?
4. **capacityPlanned** — Productive hours calculated (4-5/day), WIP limits set, utilization target 70-80%?
5. **outcomesAligned** — Deliverable-based, SMART criteria, acceptance conditions, stakeholder value stated?

### Why It Works

- **Tool calls are obligations.** The agent cannot ignore a schema that demands PERT calculations and dependency graphs.
- **The commit pattern.** The agent proposes its own verdict, then the server validates it against the pivots.
- **Semantic traps.** The engine catches task-planning anti-patterns: 'all high priority,' 'no dependencies,' 'should take about,' 'team can handle it,' 'complete the task.'


## Available Tools
- **validate_task_organization**: (1) PRIORITY — Eisenhower matrix (urgent vs important), forced ranking (only 1 is #1), ICE scoring (Impact × Confidence × Ease), cost of delay ($/day of not doing this), (2) DEPENDENCIES — blocking chains (A must finish before B starts), critical path (longest sequential chain determines project duration), parallelism (which tasks can overlap), resource conflicts (same person needed for two parallel tasks), external blockers (permits, vendors), (3) ESTIMATION — three-point (Optimistic/Most Likely/Pessimistic), PERT formula: (O + 4M + P) / 6, standard deviation: (P - O) / 6, complexity factors (new technology +50%, team inexperience +30%, external dependencies +40%), historical calibration (what similar task actually took last time), buffer (add 20-30% to PERT), (4) CAPACITY — productive hours per day: 4-5 (not 8). Context switch cost: 23 minutes per interruption (Gloria Mark, UC Irvine). WIP limits: 2-3 concurrent tasks maximum per person. Target utilization: 70-80% (not 100%). 20-30% absorbs variability and unexpected work, (5) OUTCOMES — deliverable-based (not activity-based). SMART criteria: Specific, Measurable, Achievable, Relevant, Time-bound. Acceptance criteria: what does "done" look like? Who signs off? Stakeholder value: why does this deliverable matter? Weekly review cadence.

Structured reflection tool for disciplined task organization — forces systematic priority classification, dependency mapping, estimation rigor, capacity awareness, and outcome alignment. Based on critical path method (DuPont, 1957), PERT estimation (US Navy Polaris project, 1958), Eisenhower matrix, and Goldratt's Theory of Constraints. Catches Priority Blindness (everything is marked "high priority" — nothing is actually prioritized — a hospital has 12 improvement projects, all labeled "Priority 1 — Critical." If everything is critical: nothing is critical. Staff cannot work on 12 projects simultaneously. Result: all 12 projects are 15-25% complete after 6 months. None delivered value. Fix: forced ranking. Only 1 project is #1. Apply ICE scoring: Impact (patient safety improvement) × Confidence (evidence strength) × Ease (resource availability). Rank all 12. Execute top 3 sequentially. Defer the rest. After 6 months: 3 projects 100% complete, delivering value. 9 projects queued with clear start dates), Dependency Ignorance (treating tasks as a flat list instead of a dependency graph — a construction project plan: "1. Frame walls. 2. Pour foundation. 3. Install plumbing. 4. Paint." Problem: you cannot frame walls before the foundation exists. You cannot paint before walls are framed. Plumbing must be roughed-in BEFORE drywall goes up. A flat list ignores these dependencies. Real dependencies: Foundation → Framing → Rough plumbing → Drywall → Paint. Foundation curing: 28 days (ACI 318 standard). This is the critical path. If foundation pours late: EVERYTHING downstream shifts by 28+ days. Parallel work: electrical rough-in can happen DURING plumbing rough-in (different crews, same phase). A flat list misses both: sequential dependencies AND parallel opportunities), Estimation Fantasy (guessing durations without data or methodology — "How long will it take?" "About 2 weeks." Based on what? "Experience." Whose experience? Which project? What complexity? PERT formula: Expected = (Optimistic + 4×Most Likely + Pessimistic) / 6. Example: redesign the hospital lobby. Optimistic: 3 weeks (everything goes perfectly, no change orders). Most Likely: 5 weeks (normal pace, 1-2 minor revisions). Pessimistic: 12 weeks (supply chain delay on custom fixtures, 3 design revisions, permit issues). PERT: (3 + 4×5 + 12) / 6 = 5.83 weeks. Standard deviation: (12-3)/6 = 1.5 weeks. 95% confidence: 5.83 + 2×1.5 = 8.83 weeks. "About 2 weeks" vs PERT's 8.83 weeks — the gut-feel estimate was off by 4.4x), Capacity Amnesia (assuming 8 hours = 8 productive hours — a factory shift is 8 hours. Manager schedules 8 hours of production tasks per worker. Reality: shift handover (15 min), morning briefing (10 min), breaks (2 × 15 min), lunch (30 min), equipment startup/shutdown (20 min), unplanned interruptions (avg 45 min/day). Productive time: 4.5 hours of an 8-hour shift — 56% utilization. Manager scheduled 8 hours of work into 4.5 hours of capacity. Tasks incomplete daily. Context switching (Gloria Mark, UC Irvine, 2004): 23 minutes to regain deep focus after interruption. If a worker is interrupted 6 times/day: 6 × 23 = 138 minutes lost to refocusing. WIP limit: no person should work on more than 2-3 concurrent tasks. Target utilization: 70-80%, not 100% — the remaining 20-30% absorbs variability), and Outcome Disconnect (planning activities instead of deliverables — "Task: research competitor pricing." This is an ACTIVITY, not an outcome. When is it done? After 1 hour of research? 1 day? 1 week? Deliverable version: "Deliver a 1-page competitive pricing matrix: 5 competitors × 3 pricing tiers, with source URLs and date captured. Due: Friday 5pm." The deliverable has: a concrete output (1-page matrix), scope (5 competitors × 3 tiers), acceptance criteria (source URLs, date), and a deadline. Activities are open-ended. Deliverables are completable and verifiable). Call once per task plan, project schedule, or sprint planning session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Task Organizer Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Here are 15 tasks for this sprint. All are high priority. They can be done in any order. Each should take about 2-4 hours. The team can handle it. Goal: complete the tasks."

**🤖 AI Agent:**
> PRIORITY_BLIND — Five failures: 'all high priority' = nothing prioritized, 'any order' = no dependencies, 'about 2-4h' = estimation fantasy, 'team can handle' = no capacity math, 'complete the tasks' = activity not outcome.

---

**👤 You:**
> "Priority: Q1 hotfix (ICE 800, delay $5K/day), Q2 auth refactor (ICE 224), Q3 status page (delegate), Q4 wiki header (eliminate). Dependencies: API→frontend→QA→deploy (18-day critical path). Parallel: docs + API. External: client approval 3-day SLA. Estimation: API PERT 22h, +50% new auth = 33h, historical 1.8× = 59h, +25% buffer = 74h. Capacity: Dev A 24h productive/wk, 18h committed = 6h free. Dev B 22h, 14h = 8h. WIP 2/dev. Outcomes: 'Deliver OAuth2+PKCE Google SSO, login <3s, tests pass, by Sprint 14. Unblocks enterprise sales.'"

**🤖 AI Agent:**
> ORGANIZATION_PROVEN — All five axes validated.

---

**👤 You:**
> "Priority: hotfix Q1, refactor Q2, 3 other tasks Q2. Dependencies: API→frontend→QA mapped. Estimation: 'API should take about 20 hours.' Capacity: 'team has enough bandwidth.' Outcome: 'finish the API work.'"

**🤖 AI Agent:**
> ESTIMATION_FANTASY — Priority and dependency pass. Estimation FAILS: 'should take about 20h' without three-point, PERT, or historical calibration. Capacity: 'enough bandwidth' without productive hours math. Outcome: 'finish the API work' is activity not deliverable.


## ❓ FAQ

**Q: Why do flat task lists fail?**
Flat lists hide blocking dependencies, treat all tasks as equal priority, and ignore capacity constraints. The critical path — the longest chain of dependent tasks — determines minimum completion time. Without mapping it, you discover blockers mid-sprint.

**Q: Why are 8 hours not 8 productive hours?**
Meetings, email, admin consume 30-50%. Productive deep work: 4-5 hours/day. Context switching costs 23 minutes per switch (UC Irvine). 5 switches/day = 2 hours lost. WIP limit: 2-3 concurrent tasks. Target 70-80% utilization — 100% causes burnout.

**Q: What is the difference between 'done' and 'finished'?**
Finished = stopped working on it. Done = meets acceptance criteria. 'Write report' is an activity. 'Deliver board-ready Q3 analysis with 3 recommendations by Friday' is an outcome with SMART criteria and clear acceptance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/task-organizer-prover](https://vinkius.com/mcp/task-organizer-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Task Organizer Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `task-organizer-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Task Organizer Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "task-organizer-prover": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
