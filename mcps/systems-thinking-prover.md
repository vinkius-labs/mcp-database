# Systems Thinking Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/systems-thinking-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [reasoning](../categories/reasoning.md)

AI thinks in straight lines. This engine is a 6-pivot cognitive trap that forces the LLM to map feedback loops, second-order effects, and bottlenecks before proposing any architectural change.

## Description
LLMs think in straight lines (A causes B). They fail to see feedback loops (A causes B, which causes more A). The Systems Thinking Prover is a cognitive trap designed to break linear thinking.

### The Semantic Trap

Before outputting a solution, the agent must pass a strict 6-pivot validation:

1. **systemBoundariesMapped** — What is the scope of the system?
2. **feedbackLoopsIdentified** — Where are the reinforcing/balancing loops?
3. **secondOrderEffectsTraced** — What happens downstream?
4. **bottlenecksIsolated** — Where is the actual constraint?
5. **unintendedConsequences** — How will this break unexpectedly?
6. **mathChecksOut** — Prove the throughput math.


## Available Tools (1)
- **validate_systems_thinking**: Include every node that receives output from your system. If the traffic light's boundary excludes adjacent intersections: the boundary is wrong, (2) FEEDBACK LOOPS — identify EVERY reinforcing (amplifying) and balancing (stabilizing) loop. Reinforcing: more boats → fewer fish → more boats (spiral). Balancing: fish reproduction → population recovery → sustainable harvest (equilibrium). Name each loop. Classify it. Trace its path, (3) SECOND-ORDER EFFECTS — trace at least 3 orders of consequences. For each first-order effect: "and then what happens?" Repeat 3x minimum. Hospital beds → faster admission → more patients → worse care → lawsuits, (4) BOTTLENECK — identify the ONE constraint (Goldratt's TOC). Throughput = capacity of the constraint, not the fastest component. All investment should target the constraint until it is no longer the constraint, (5) UNINTENDED CONSEQUENCES — what will break that you did not intend to affect? Who loses when your intervention succeeds? What incentive does it create?, (6) MATH — prove the system capacity with numbers. Throughput = min(capacity of each stage). If intervention does not change the min: output is unchanged. If rejected, your intervention will make the system worse.

Structured reflection tool that forces the LLM to map second-order effects and feedback loops BEFORE proposing any system change. Based on Donella Meadows' "Thinking in Systems" (2008), Jay Forrester's System Dynamics (MIT), and the 12 leverage points framework. Systems thinking prevents the most common reasoning failure: intervening in a complex system without understanding the feedback loops that will amplify, dampen, or reverse your intervention. Catches Scope Neglect (drawing system boundaries too narrowly — missing connected subsystems — a city installs a new traffic light at a congested intersection. Boundary drawn: the single intersection. Intervention: 90-second green cycle for the main road. Result at the intersection: congestion reduced 40%. "Success!" Result at the 3 adjacent intersections: congestion INCREASED 60% — cars now flow faster into the next bottleneck, which has the same capacity as before. Total system congestion: increased 15%. The intervention made the SYSTEM worse. The boundary was drawn too narrowly. The system is not one intersection — it is a road network. Fix: model the entire corridor (5+ intersections) with synchronized light timing. Adaptive signal control: lights coordinate to create "green waves" along the corridor. Rule: if your boundary excludes any node that receives output from your system, the boundary is wrong), Linear Thinking (assuming cause and effect are proportional — ignoring feedback loops — a fishing village increases its fleet by 30% to catch 30% more fish. Year 1: catch increases 25%. Revenue up. More boats ordered. Year 2: catch increases only 10% — fish population declining. Even more boats ordered to compensate. Year 3: catch DECREASES 15% — fish population collapsing under overharvesting. Year 5: fishery collapses entirely. Zero catch. This is a reinforcing loop (more boats → fewer fish → more boats to compensate → even fewer fish) interacting with a balancing loop (fish reproduction rate — which has a maximum capacity). When the harvesting rate exceeds the reproduction rate: the balancing loop cannot compensate. The system has a tipping point — and it was crossed silently in Year 2. Linear thinking: 30% more boats = 30% more fish. Systems thinking: 30% more boats may = 0% more fish. Fix: identify the BALANCING LOOP (fish reproduction rate) and ensure harvesting stays below its capacity), Second-Order Blindness (seeing only the immediate effect, not the cascading consequences — a hospital reduces ER wait times by adding 10 more beds. First-order effect: patients are admitted faster. Wait time: 4 hours → 2 hours. Second-order effect: faster admission → word spreads → more patients come to this ER (they drive PAST other hospitals because "this ER is fast"). Volume increases 35%. Third-order effect: 10 more beds with same number of nurses and doctors → staff-to-patient ratio degrades → quality of care drops → medical errors increase 22%. Fourth-order effect: medical errors → lawsuits → insurance premiums increase → budget cuts → staff reduction. The intervention that "reduced wait times" ultimately INCREASED wait times AND reduced care quality. Fix: trace at least 3 orders of effects before implementing. For each effect, ask: "and then what happens?" until you reach the system boundary), Bottleneck Misidentification (optimizing a non-constraint — Goldratt's Theory of Constraints — a bakery can mix 200 batches/day, proof 150 batches/day, and bake 180 batches/day. Management invests $50K in a faster mixer: now mixes 300 batches/day. Total output: still 150 batches/day. The mixer was never the bottleneck — proofing is. The $50K investment produced exactly $0 in additional output. Eliyahu Goldratt (The Goal, 1984): the throughput of a system is determined by ONE constraint. Optimizing a non-constraint is waste — the system output does not change. Fix: identify the constraint (proofing: 150 batches/day). All improvements target the constraint. Options: second proofing room ($30K), stagger proofing schedule (free), reduce proofing time (process improvement). Only AFTER proofing exceeds 180 does the oven become the new constraint), and Naive Intervention (changing a variable without understanding delay and oscillation — a farmer irrigates a field. Soil moisture sensor reads 20% (too dry). Farmer opens the irrigation valve fully. Waits 1 hour. Sensor still reads 22% (barely changed). "Not enough water!" Opens a second valve. Problem: water takes 4-6 hours to permeate through the soil to the sensor depth. After 6 hours: soil moisture reads 85% — severely overwatered. Roots drowning. Crop damage. This is a DELAY in the feedback loop. The sensor gives accurate but DELAYED information. The farmer's intervention was based on the delay, not the system state. Same pattern in every system: central banks raise interest rates, but economic effects lag 12-18 months — leading to overcorrection (raise too much, then cut too much). Fix: identify the delay in your feedback loop BEFORE intervening. If the delay is 4 hours: wait 4 hours after intervention before measuring effect. Small interventions with wait periods > oscillating large interventions). Call once per system change, policy decision, or complex intervention


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Systems Thinking Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Boundaries: App server. Loop: none. Second order: faster app."

**🤖 AI Agent:**
> Verdict: LINEAR_THINKING_DETECTED. You failed to identify reinforcing or balancing feedback loops in the system.

---

**👤 You:**
> "Loop: balancing loop on DB. Second order: none. Bottleneck: DB."

**🤖 AI Agent:**
> Verdict: SECOND_ORDER_BLINDNESS. You failed to trace the downstream effects. What happens when the DB bottleneck is removed?

---

**👤 You:**
> "Loop: Reinforcing loop on cache hits. Second order: Primary DB gets cold. Bottleneck: Redis CPU. Unintended: Cache stampede. Math: 5k RPS limit."

**🤖 AI Agent:**
> Verdict: SYSTEMS_THINKING_PROVEN. You mapped the loops, traced the cold DB effect, and isolated the real constraint.


## ❓ FAQ

**Q: Why force the identification of feedback loops?**
Systems are not linear. If you fix a bottleneck without mapping the reinforcing loop, the system will just break faster somewhere else.

**Q: What is a second-order effect?**
The consequence of the consequence. Fixing the DB makes the app faster, which draws more users, which crashes the cache.

**Q: How do you prove math in systems thinking?**
By calculating throughput, capacity, or latency limits (e.g. proving a 5k RPS upstream source will crash a 1k RPS bottleneck database).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/systems-thinking-prover](https://vinkius.com/mcp/systems-thinking-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Systems Thinking Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `systems-thinking-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Systems Thinking Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "systems-thinking-prover": {
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
