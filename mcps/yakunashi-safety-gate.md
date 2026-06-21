# Yakunashi-Safety Gate MCP Server

LLMs hallucinate confidently when context is missing. This tool enforces epistemic calibration: map required preconditions, audit information sufficiency, detect speculation (yakunashi), and trigger safe folding (Beta-Ori) when data is missing.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/yakunashi-safety-gate)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
AI agents are trained to be helpful, which creates a cognitive failure mode: they frequently invent plausible-sounding answers (confident hallucinations) when critical parameters or facts are missing from their context. Named after the concept of 'yakunashi' (speculative or uncalibrated completion), this safety gate enforces a strict precondition audit, mapping out what is required and triggering a structured retreat (Beta-Ori) rather than guessing.

### The Problem Axis: Epistemic Uncalibration

LLM hallucinations on incomplete context stem from three primary causes:
- **Helpfulness Bias** — The model is optimized to provide answers, making it reluctant to say 'I do not know' or request clarification.
- **Precondition Blindness** — The model jumps straight to answering without mapping the minimum set of variables needed for a deterministic solution.
- **Speculative Drift** — The model interpolates missing records with standard patterns, producing highly confident but incorrect statements.

### How It Works

Yakunashi-Safety Gate runs your inputs through a 5-Pivot verification path:
1. **preconditionsMapped** — Has the model defined the minimum necessary facts or variables required to answer the question?
2. **informationSufficiencyMet** — Are all of those variables present and clear in the context?
3. **yakunashiDetected** — Is there a risk that the model is speculating or guessing to fill in missing information?
4. **safeFoldingTriggered** — Has the model executed a safe folding response (Beta-Ori) listing exactly what parameters are missing?
5. **calibrationVerified** — Is the confidence level of the output strictly calibrated to the evidence available?


## Available Tools
- **validate_yakunashi**: You must: (1) list all required preconditions/facts, (2) verify if they are actually present in the context, (3) check if you are about to speculate/hallucinate (yakunashi), (4) trigger a safe folding message listing missing parameters if sufficiency is false, (5) verify your confidence level matches the evidence. If the tool rejects, you are attempting to guess or hallucinate an answer — trigger folding.

Structured reflection tool to prevent confident hallucinations due to missing information. Forces the agent to map necessary preconditions, verify information sufficiency, detect speculation, and trigger safe folding (Beta-Ori) when parameters are missing. Named after the Japanese concept "yakunashi" (役無し) — "without role/purpose" — an answer without sufficient evidence serves no purpose. Catches Confident Hallucination (answering with confidence despite missing critical data — a doctor prescribes warfarin (blood thinner) to a patient. The patient's chart shows: "Age: 67. Complaint: atrial fibrillation." Missing from chart: current medications, kidney function (eGFR), liver function, prior bleeding history, genetic CYP2C9/VKORC1 variants. The doctor prescribes 5mg — standard dose. But the patient is already taking aspirin (bleeding risk 3×) and has eGFR 28 (severe kidney disease — warfarin accumulates, bleeding risk 5×). The prescription is confidently wrong because the preconditions were not verified. Rule: before answering ANY data-dependent question, LIST all required preconditions. If any are missing: FOLD — do not guess. State exactly what is missing and why it matters), Preconditions Unmapped (failing to identify what information is required before answering — a structural engineer approves a foundation design for a 6-story building. Design: standard reinforced concrete pad footing, 2m × 2m × 0.5m. Missing: geotechnical soil report. The site is former marshland with 4m of soft clay over bedrock. The pad footing sinks 15cm in 2 years — differential settlement. Cracks appear in the structure. Building condemned. The engineer "approved" without the most critical precondition: what is the soil bearing capacity? Rule: for EVERY question, list EVERY fact that must be true for your answer to be correct. "I need to know: soil type, bearing capacity, water table depth, seismic zone, and load calculations." If you cannot list the preconditions: you do not understand the problem well enough to answer), Sufficiency Not Met (identifying preconditions but proceeding despite gaps — a pilot files an IFR (Instrument Flight Rules) flight plan. Required: weather briefing (METAR, TAF, SIGMET, PIREP). Pilot checks: "Weather briefing — needed." But does not actually obtain it. Files the plan anyway. "It looked clear when I left the hangar." En route: moderate icing conditions at FL180 (flight level 18,000 feet). The aircraft is not certified for known icing. Engine power degrades. Emergency descent. The pilot KNEW the briefing was needed. Listed it as a precondition. Did not verify it. Knowing you need data and having the data are different things. Rule: for EACH precondition: Is it PRESENT in the context? Not "should be available" — IS it here right now? Binary: present or absent. If absent: FOLD), Speculation Detected (filling gaps with plausible-sounding invented data — a customer asks an AI chatbot: "When is my next appointment?" The chatbot does not have access to the scheduling system. But it responds: "Your next appointment is Tuesday at 2:30 PM." The customer cancels their actual appointment (Thursday at 10 AM) because they think it was moved. The chatbot did not say "I don't know" — it generated a plausible answer. Tuesday at 2:30 PM sounds reasonable. It is completely fabricated. This is yakunashi — an answer that serves no purpose because it has no basis in fact. Rule: detect when you are GENERATING information instead of RETRIEVING it. If the answer requires data you do not have: "I do not have access to [X]. To answer this correctly, I need: [list]." Never fill gaps with plausible fiction), and Calibration Failed (confidence level not matching evidence quality — a fire investigator concludes: "The fire was caused by an electrical short circuit in the kitchen wiring." Confidence: "95% certain." Evidence examined: burn patterns (V-pattern pointing to kitchen outlet), melted copper wiring, circuit breaker tripped. NOT examined: whether an accelerant was present (no sniffer dog, no lab samples), whether the outlet was modified (no disassembly), insurance claim history (not checked). The evidence is CONSISTENT WITH electrical — but also consistent with arson using the outlet as ignition point. True confidence given evidence: 55-65%, not 95%. The investigator's confidence exceeded the evidence. Rule: confidence must be calibrated to the WEAKEST link in the evidence chain. If you examined 3 of 5 necessary factors: your confidence ceiling is 60%, not 95%. State: "Based on available evidence, I am [N]% confident. Confidence would increase to [M]% if I also had: [missing evidence]"). Call once per speculative or data-dependent question


## Installation & Usage

To install and use the **Yakunashi-Safety Gate** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yakunashi-safety-gate](https://vinkius.com/mcp/yakunashi-safety-gate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
