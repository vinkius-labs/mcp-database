# Watt Efficiency Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/watt-efficiency-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [complex-reasoning](../categories/complex-reasoning.md)

A team spent 6 weeks 'optimizing' their operation. No baseline. No analysis. They restructured the most visible department. Processing time got worse. The bottleneck was a manual approval step in a different department — untouched entire time. Watt measured the Newcomen engine and found 80% of steam energy wasted reheating the cylinder. He did not 'optimize the engine' — he measured, identified, and eliminated specific waste. This tool forces that discipline: identify waste with data, instrument baselines, design feedback, isolate the bottleneck, and quantify improvement with numbers.

## Description
Agents propose optimizations without measuring anything. They say 'make it faster' without knowing what is slow. They optimize the wrong component. They claim 'significant improvement' without a single number.

### The Problem

LLMs commit five efficiency failures:

- **Waste Unidentified** — 'We should optimize the process.' Optimize what? Which step? Which stage within that step? What resource is being wasted — time? Materials? Labor? Capital? Watt measured the Newcomen engine and found 80% of steam energy was lost reheating the cylinder after every stroke. Not 'the engine is inefficient' — '80% of energy is lost HERE, in the cylinder cooling cycle, because steam condenses on cold metal walls.' WHERE is YOUR 80%?
- **Measurement Absent** — 'The process feels slow.' Feels. Not IS. Watt invented the indicator diagram — a mechanical device that traced pressure vs. volume inside the cylinder during every stroke. Real-time instrumentation. What is your actual cycle time? Measured by what method? At what volume? Under what conditions? Before and after — same conditions, direct comparison.
- **Feedback Missing** — 'We review the reports every morning.' That is not a feedback loop. Watt's centrifugal governor is: when the engine speeds up, the spinning weights rise and restrict steam flow. When it slows down, weights drop and open the valve. Automatic. No engineer in the loop. Does your system auto-adjust when demand rises? Does it throttle when errors spike? Does it shed load when queues grow? With damping to prevent oscillation?
- **Bottleneck Misidentified** — 'Let us restructure the visible department.' That department takes 12 minutes. The hidden approval step takes 340 minutes. You are optimizing 3% of the total cycle time. Watt identified the cylinder — not the boiler, not the piston, not the beam. He analyzed the system and found the SINGLE component where energy was lost. Run your analysis. Map the process. Name the ONE constraint.
- **Efficiency Unquantified** — 'It is much faster now.' How much? 10%? 90%? Compared to what baseline? What did the optimization cost? Watt DEFINED horsepower — 33,000 foot-pounds per minute — so customers could COMPARE engines with a number, not an adjective.

### How It Works

5 Decision Pivots following Watt's methodology:

1. **wasteIdentified** — Specific resource, exact waste point, measured magnitude, root cause.
2. **measurementInstrumented** — Baseline metric before, measurement method, granularity, after metric.
3. **feedbackDesigned** — Signal, threshold, automatic action, damping mechanism.
4. **bottleneckIsolated** — Analyzed critical path, single constraint with evidence, post-fix shift.
5. **efficiencyQuantified** — Before/after exact metrics, percentage improvement, optimization cost.

### The Verdict Matrix

| First Failing Pivot | Verdict | Meaning |
|---|---|---|
| wasteIdentified = false | WASTE_UNIDENTIFIED | Optimizing without measuring waste. |
| measurementInstrumented = false | MEASUREMENT_ABSENT | No baseline, no instrument. |
| feedbackDesigned = false | FEEDBACK_MISSING | No automatic self-correction. |
| bottleneckIsolated = false | BOTTLENECK_MISIDENTIFIED | Optimizing the wrong component. |
| efficiencyQuantified = false | EFFICIENCY_UNQUANTIFIED | "Faster" without numbers. |
| All pivots pass | EFFICIENCY_PROVEN | Waste found. Measured. Feedback. Isolated. Quantified. |


## Available Tools
- **validate_watt_efficiency**: You must: (1) MEASURE — energy in vs. work out, precise input/output ratio, not "should be faster," (2) IDENTIFY WASTE — where resources are consumed without producing value, (3) QUANTIFY COST OF CHANGE — investment, downtime, transition risk, training, disruption, (4) PROVE GAINS — before/after measurements with the same methodology, (5) PRESERVE OUTPUT — efficiency must not degrade quality, safety, or reliability. If rejected, fix the specific efficiency gap the engine identifies.

Structured reflection tool that forces the LLM to think like James Watt — measure resource efficiency with precision, identify waste in every process, quantify the cost of change versus the cost of status quo, prove efficiency gains with measured before/after data, and preserve output quality during optimization. Watt did not invent the steam engine — he measured why Newcomen's engine wasted 75% of its heat, then engineered a separate condenser that recovered that energy. The breakthrough was not invention — it was measurement. Catches Efficiency Unmeasured (claiming improvement without measuring input/output ratio — a textile mill in 1780: "Our new steam engine is better than the old one." Better how? "It feels more powerful." Watt's approach: measure coal consumed (input) per bales of cotton processed (output). Old engine: 12 lbs of coal per bale. New engine: 4.5 lbs per bale. That is a 62.5% efficiency gain — measured, not felt. Without measurement: the mill owner cannot know if the £400 investment was justified. Modern equivalent: a hospital claims "our new scheduling system is more efficient." Efficient how? How many patients per hour before? After? What changed? Rule: state the precise input/output ratio before AND after — "$47 per unit produced" or "2.3 hours per case resolved" — not "faster" or "better"), Waste Unidentified (optimizing the wrong thing because waste was never mapped — a hospital operating room: surgeons complain about long turnover times between surgeries. Administration buys faster sterilization equipment — $120,000. Turnover time: unchanged. Why? Because 70% of turnover time was NOT sterilization. It was: waiting for the next patient to arrive from pre-op (18 minutes). Surgeon doing pre-op paperwork that a nurse could complete (12 minutes). Anesthesiologist arriving late because they were checking another patient (15 minutes). The sterilization was 8 minutes. It was never the bottleneck. $120,000 spent. Problem unchanged. Because no one MAPPED where time was actually lost. Watt's waste taxonomy: WAIT (idle time — materials, people, decisions queued). DUPLICATION (same work done twice — same data in 3 systems). OVERPRODUCTION (more than needed — reports nobody reads, inventory above demand). DEFECTS (rework — returns, corrections, failed inspections). Map ALL four before optimizing ANY one), Change Cost Unknown (implementing improvement without calculating total cost of transition — a bakery owner: "A new convection oven will bake croissants 30% faster!" Cost: $40,000. Current oven bakes 200 croissants/hour. New oven: 260/hour. Croissant profit margin: $0.85 each. Extra 60 croissants/hour × $0.85 = $51/hour. Bakery operates 8 hours/day, 25 days/month = $10,200/month extra revenue. But wait — can the bakery SELL 60 extra croissants/hour? Current demand: 180/hour. The oven already exceeds demand. The new oven bakes 260 for a market of 180. The $40,000 oven produces unsold croissants. ROI: never. The bottleneck was demand, not baking speed. Rule: quantify investment, downtime during transition, risk if it fails, AND verify the bottleneck is what you think it is), Improvement Unproven (claiming gains without before/after measurement with identical methodology — a factory manager: "Since the new layout, production is up 20%!" Measured how? "July output was 12,000 units. December output is 14,400 units." But July had 3 weeks of vacation absences. December is peak season with overtime. Same methodology? No. Same conditions? No. The "improvement" is seasonal variation, not layout effect. Watt's method: measure coal per horsepower-hour. Same fuel. Same engine. Same load. Before condenser: 30 lbs/hp-hr. After: 7.5 lbs/hp-hr. Same conditions. Single change. Rule: before/after must use identical methodology, identical conditions, and single change — if you changed 5 things simultaneously, you cannot attribute the result to any one), and Output Degraded (improving efficiency at the expense of quality, safety, or reliability — a clinic reduces appointment times from 12 minutes to 8 minutes. Efficiency: patients per hour increases from 5 to 7.5 — a 50% improvement! But: misdiagnosis rate doubles. Patient satisfaction drops from 4.2/5 to 2.8/5. Complaints to the medical board: 3 per quarter → 11 per quarter. The clinic is "more efficient" at producing worse outcomes. Watt's separate condenser improved BOTH efficiency AND output stability — the engine ran smoother AND used less coal. Efficiency that degrades output is not optimization — it is cutting corners. Rule: measure quality metrics before and after. If quality dropped: the "efficiency" is fake). Call once per optimization, cost-reduction, or process improvement proposal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Watt Efficiency Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Our process is slow and we need to make it faster. We should optimize the whole operation. Clients are complaining about delivery time."

**🤖 AI Agent:**
> WASTE_UNIDENTIFIED — 'The process is slow,' 'make it faster,' 'optimize the whole operation' — three sentences, zero measurements. Watt did not 'optimize the engine.' He measured the Newcomen engine and found 80% of steam energy was lost reheating the cylinder. WHERE is YOUR waste? Which step is slow? Which stage within that step? Is it waiting time? Processing time? Transport time? Rework? What is the actual cycle time? 'Clients are complaining' is an anecdote, not a waste analysis. Measure before you touch anything.

---

**👤 You:**
> "Waste: Order fulfillment step — average cycle time 340 minutes. 73% of total time is in manual quality inspection (248 min of 340 min). The inspection requires checking each item against a 47-point checklist manually because the checklist was never digitized — no structured template exists. Assembly and packaging are under 15% of total time. Measurement: Baseline average = 340 min (time study, 7-day average, volume: 850 orders/day). After introducing structured digital checklist with auto-pass for standard items: average = 92 min (same time study method, same volume, measured 48h post-implementation). Granularity: per-order via tracking system. Feedback: Signal: average cycle time per order. Threshold: > 150 min for 3 consecutive batches. Action: automatic workload redistribution to backup inspection team. If > 250 min for 10 consecutive orders: escalate to operations lead with root cause triage. If > 400 min for 5 consecutive: halt non-critical orders, focus resources on clearing backlog. Damping: 15-minute cooldown between redistribution events, stand-down requires 30 minutes of cycle time < 100 min. Bottleneck: Process analysis (time study, 10 consecutive orders during peak): 73% of cycle time in manual checklist verification. After digital checklist: next bottleneck shifts to packaging — 34 min (37% of new 92 min total), identified via same time study. Efficiency: Before: avg = 340 min, inspection = 248 min (73%). After: avg = 92 min, inspection = 18 min (20%). Improvement: 73% cycle time reduction (340 → 92 min), inspection 93% faster (248 → 18 min). Cost: 2 days implementation (digital template creation, staff training took 47 minutes, zero production downtime via parallel rollout). Tradeoff: digital system adds monthly subscription cost, training overhead for new staff increases by ~2 hours per onboarding."

**🤖 AI Agent:**
> EFFICIENCY_PROVEN — Watt Method complete. Waste: order fulfillment, 73% of 340 min cycle time spent in manual 47-point checklist verification — resource (labor), location (quality inspection stage), magnitude (248 min of 340 min), cause (no structured digital template). Measurement: time study baseline 340 min → 92 min post-implementation, same volume (850 orders/day), per-order tracking. Feedback: 3-tier automatic response (redistribute at >150 min, escalate at >250 min, halt non-critical at >400 min) with 15-minute cooldown damping. Bottleneck: time study proves 73% in manual checklist. Post-fix shift to packaging (34 min, 37%) documented. Efficiency: 73% cycle time reduction, 93% inspection speedup, 2 days implementation cost, subscription tradeoff, 2-hour training overhead. This is measured improvement, not hand-waving.

---

**👤 You:**
> "Waste: 73% of cycle time in quality inspection. Measurement: baseline 340 min via time study. Feedback: we review the reports every morning and someone monitors it during peak hours. Bottleneck: quality inspection is always the bottleneck — it must be the checklists."

**🤖 AI Agent:**
> FEEDBACK_MISSING — Waste and measurement pass: 73% in quality inspection, 340 min baseline via time study — good. But feedback fails: 'we review reports every morning' and 'someone monitors during peak hours' are reactive human monitoring, not feedback loops. Watt's centrifugal governor adjusts AUTOMATICALLY — no engineer in the loop. What happens on a holiday weekend when nobody is reviewing reports and cycle time spikes to 800 minutes? Define: signal (average cycle time per order), threshold (> 150 min for 3 consecutive batches), automatic action (redistribute workload, escalate at 250 min), damping (15-minute cooldown). Also: 'quality inspection is always the bottleneck' — WHICH checks? WHICH items? Manual verification or automated checks? Process analysis or gut feeling?


## ❓ FAQ

**Q: Is this only for operations performance?**
No. Watt's method applies to any system where resources are consumed and efficiency matters — manufacturing throughput, service delivery speed, administrative processing time, supply chain turnaround, team productivity, budget utilization, equipment uptime. The 5 pivots — waste identification, measurement, feedback, bottleneck isolation, quantification — work wherever you can measure input vs. useful output.

**Q: What counts as a valid feedback loop?**
Four elements: (1) a SIGNAL — a metric that indicates drift (cycle time rising, defect rate climbing, queue growing), (2) a THRESHOLD — a specific value that triggers action (cycle time > 200 minutes for 3 consecutive batches), (3) an AUTOMATIC ACTION — something that happens without human intervention (reallocate resources, activate backup capacity, redistribute workload), (4) DAMPING — a mechanism to prevent oscillation (cooldown period, gradual scaling, minimum stable period before further changes). 'We check reports' is monitoring. Watt's centrifugal governor is a feedback loop — it adjusts without an engineer.

**Q: How does it differ from the Brunel Engineering Prover?**
Brunel validates engineering at SCALE — what breaks at 10x/100x, integration contracts, specification tolerances, risk quantification, precedent challenge. Watt validates EFFICIENCY — where waste occurs, measurement instrumentation, feedback control, bottleneck isolation, quantified improvement. Brunel asks 'will this survive growing 10x?' Watt asks 'where is 80% of your resources being wasted right now, and can you prove the optimization worked?' Use Brunel for scale planning, Watt for performance tuning.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/watt-efficiency-prover](https://vinkius.com/mcp/watt-efficiency-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Watt Efficiency Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `watt-efficiency-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Watt Efficiency Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "watt-efficiency-prover": {
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
