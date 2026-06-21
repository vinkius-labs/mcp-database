# Watt Efficiency Prover MCP Server

A team spent 6 weeks 'optimizing' their operation. No baseline. No analysis. They restructured the most visible department. Processing time got worse. The bottleneck was a manual approval step in a different department — untouched entire time. Watt measured the Newcomen engine and found 80% of steam energy wasted reheating the cylinder. He did not 'optimize the engine' — he measured, identified, and eliminated specific waste. This tool forces that discipline: identify waste with data, instrument baselines, design feedback, isolate the bottleneck, and quantify improvement with numbers.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/watt-efficiency-prover)

## Overview
**Category:** complex-reasoning
**Tools Count:** 1

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


## Installation & Usage

To install and use the **Watt Efficiency Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/watt-efficiency-prover](https://vinkius.com/mcp/watt-efficiency-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
