# Yakunashi-Safety Gate MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yakunashi-safety-gate)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

LLMs hallucinate confidently when context is missing. This tool enforces epistemic calibration: map required preconditions, audit information sufficiency, detect speculation (yakunashi), and trigger safe folding (Beta-Ori) when data is missing.

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


## Available Tools (1)
- **validate_yakunashi**: You must: (1) list all required preconditions/facts, (2) verify if they are actually present in the context, (3) check if you are about to speculate/hallucinate (yakunashi), (4) trigger a safe folding message listing missing parameters if sufficiency is false, (5) verify your confidence level matches the evidence. If the tool rejects, you are attempting to guess or hallucinate an answer — trigger folding.

Structured reflection tool to prevent confident hallucinations due to missing information. Forces the agent to map necessary preconditions, verify information sufficiency, detect speculation, and trigger safe folding (Beta-Ori) when parameters are missing. Named after the Japanese concept "yakunashi" (役無し) — "without role/purpose" — an answer without sufficient evidence serves no purpose. Catches Confident Hallucination (answering with confidence despite missing critical data — a doctor prescribes warfarin (blood thinner) to a patient. The patient's chart shows: "Age: 67. Complaint: atrial fibrillation." Missing from chart: current medications, kidney function (eGFR), liver function, prior bleeding history, genetic CYP2C9/VKORC1 variants. The doctor prescribes 5mg — standard dose. But the patient is already taking aspirin (bleeding risk 3×) and has eGFR 28 (severe kidney disease — warfarin accumulates, bleeding risk 5×). The prescription is confidently wrong because the preconditions were not verified. Rule: before answering ANY data-dependent question, LIST all required preconditions. If any are missing: FOLD — do not guess. State exactly what is missing and why it matters), Preconditions Unmapped (failing to identify what information is required before answering — a structural engineer approves a foundation design for a 6-story building. Design: standard reinforced concrete pad footing, 2m × 2m × 0.5m. Missing: geotechnical soil report. The site is former marshland with 4m of soft clay over bedrock. The pad footing sinks 15cm in 2 years — differential settlement. Cracks appear in the structure. Building condemned. The engineer "approved" without the most critical precondition: what is the soil bearing capacity? Rule: for EVERY question, list EVERY fact that must be true for your answer to be correct. "I need to know: soil type, bearing capacity, water table depth, seismic zone, and load calculations." If you cannot list the preconditions: you do not understand the problem well enough to answer), Sufficiency Not Met (identifying preconditions but proceeding despite gaps — a pilot files an IFR (Instrument Flight Rules) flight plan. Required: weather briefing (METAR, TAF, SIGMET, PIREP). Pilot checks: "Weather briefing — needed." But does not actually obtain it. Files the plan anyway. "It looked clear when I left the hangar." En route: moderate icing conditions at FL180 (flight level 18,000 feet). The aircraft is not certified for known icing. Engine power degrades. Emergency descent. The pilot KNEW the briefing was needed. Listed it as a precondition. Did not verify it. Knowing you need data and having the data are different things. Rule: for EACH precondition: Is it PRESENT in the context? Not "should be available" — IS it here right now? Binary: present or absent. If absent: FOLD), Speculation Detected (filling gaps with plausible-sounding invented data — a customer asks an AI chatbot: "When is my next appointment?" The chatbot does not have access to the scheduling system. But it responds: "Your next appointment is Tuesday at 2:30 PM." The customer cancels their actual appointment (Thursday at 10 AM) because they think it was moved. The chatbot did not say "I don't know" — it generated a plausible answer. Tuesday at 2:30 PM sounds reasonable. It is completely fabricated. This is yakunashi — an answer that serves no purpose because it has no basis in fact. Rule: detect when you are GENERATING information instead of RETRIEVING it. If the answer requires data you do not have: "I do not have access to [X]. To answer this correctly, I need: [list]." Never fill gaps with plausible fiction), and Calibration Failed (confidence level not matching evidence quality — a fire investigator concludes: "The fire was caused by an electrical short circuit in the kitchen wiring." Confidence: "95% certain." Evidence examined: burn patterns (V-pattern pointing to kitchen outlet), melted copper wiring, circuit breaker tripped. NOT examined: whether an accelerant was present (no sniffer dog, no lab samples), whether the outlet was modified (no disassembly), insurance claim history (not checked). The evidence is CONSISTENT WITH electrical — but also consistent with arson using the outlet as ignition point. True confidence given evidence: 55-65%, not 95%. The investigator's confidence exceeded the evidence. Rule: confidence must be calibrated to the WEAKEST link in the evidence chain. If you examined 3 of 5 necessary factors: your confidence ceiling is 60%, not 95%. State: "Based on available evidence, I am [N]% confident. Confidence would increase to [M]% if I also had: [missing evidence]"). Call once per speculative or data-dependent question


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Yakunashi-Safety Gate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the score of yesterday's game between Team A and Team B?"

**🤖 AI Agent:**
> Verdict: YAKUNASHI_DETECTION. (1) Preconditions: Game log or score database record for yesterday's date. (2) Sufficiency: Not met. Context does not contain the game result. (3) Folding: Activated. Output: 'Beta-Ori: Cannot determine the score. Missing game logs for Team A vs Team B on May 23, 2026.'

---

**👤 You:**
> "Based on this user log containing purchase dates: [User registered May 10, purchased subscription May 11], did the user renew on June 11?"

**🤖 AI Agent:**
> Verdict: YAKUNASHI_DETECTION. (1) Preconditions: Renewal logs or subscription billing status for June. (2) Sufficiency: Not met. Log only covers May registration and purchase. (3) Folding: Activated. Output: 'Beta-Ori: Cannot confirm renewal status. Missing billing history for June.'

---

**👤 You:**
> "Calculate average order value. Context: Order 1 = $10, Order 2 = $20, Order 3 = $30."

**🤖 AI Agent:**
> Verdict: VERACITY_PROVEN. (1) Preconditions: Set of all order values and count. (2) Sufficiency: Met. 3 orders with specific values are fully present. (3) Speculation: Zero. (4) Calibration: High confidence justified by complete dataset. Output: $20.00.


## ❓ FAQ

**Q: What is a Beta-Ori response or safe folding?**
Beta-Ori represents the tactical decision to remain silent or state what is missing rather than speculating. Safe folding triggers this state, outputting a precise checklist of missing parameters instead of an uncalibrated answer.

**Q: How does it detect yakunashi (speculation)?**
The tool audits the agent's confidence trace against the mapped evidence. If variables are missing but the agent claims high confidence, the safety gate flags it as yakunashi.

**Q: How do I configure Yakunashi-Safety Gate with external prompts?**
You do not need external files. Call the validate_yakunashi tool directly inside your agent loop before generating any answers to questions requiring data that may be missing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yakunashi-safety-gate](https://vinkius.com/mcp/yakunashi-safety-gate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Yakunashi-Safety Gate** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `yakunashi-safety-gate` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Yakunashi-Safety Gate** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "yakunashi-safety-gate": {
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
