# Flight Risk Assessment Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flight-risk-assessment-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [safety & compliance](../categories/safety-compliance.md)

A dispatch office cleared a flight into known CB activity with 'proceed with caution.' The crew never returned. Flight Risk Prover forces ICAO SMS-level threat identification with METAR data, 5×5 risk quantification, Swiss Cheese barrier modeling, SHELL/IMSAFE human factors analysis, and explicit GO/NO-GO commitment — eliminating the sycophantic go-bias that kills in aviation.

## Description
Flight Risk Assessment Prover enforces ICAO Safety Management System rigor across 5 axes that LLMs consistently fail:

**Axis 1 — Threat Specificity.** Generic 'weather risk' is rejected. Every threat must be named with METAR/TAF data, TEM categories (environmental, airline, crew), measurable parameters (crosswind component, RVR vs minimums, ceiling vs DA, icing level, fuel impact), and exposure duration.

**Axis 2 — Risk Quantification.** Adjective-based 'medium risk' is rejected. Each threat is scored on the ICAO 5×5 matrix: Probability (A=Extremely Improbable to E=Frequent) × Severity (1=Negligible to 5=Catastrophic). Compound risk and post-mitigation residual risk must be calculated. Index >15 is Intolerable (NO-GO).

**Axis 3 — Barrier Modeling.** 'Safety measures in place' is rejected. Swiss Cheese defense layers must be mapped: Organizational (SMS, policies) → Supervisory (dispatch, scheduling) → Preconditions (MEL items, crew fitness) → Acts (technique, monitoring). Holes identified in each layer, alignment checked across layers.

**Axis 4 — Human Factors.** 'Pilot error' is rejected. SHELL model analysis (Software-Hardware-Environment-Liveware) plus IMSAFE checklist (Illness, Medication, Stress, Alcohol, Fatigue, Eating). Fatigue quantified: hours since sleep, FDP position, WOCL exposure.

**Axis 5 — GO/NO-GO.** 'Proceed with caution' is rejected as sycophantic go-bias. Explicit GO or NO-GO with pre-defined criteria. CVR audit: 'Would I defend this decision in an investigation?'

Every lazy shortcut — generic threats, adjective risk, missing barriers, pilot blame, or go-bias — is caught by semantic traps and consistency gates before a RISK_PROVEN verdict is issued.


## Available Tools (1)
- **validate_flight_risk**: You must think like a Safety Officer at a major airline — the person whose signature means 200 people go airborne. You must: (1) identify THREATS with measured parameters — METAR/TAF data, TEM category (environmental, airline, crew), specific values (crosswind component, RVR, ceiling vs DA/MDA), exposure duration. "Weather risk" is rejected, (2) QUANTIFY risk on the ICAO 5×5 matrix — Probability (A=Extremely Improbable to E=Frequent) × Severity (1=Negligible to 5=Catastrophic) = Risk Index. Score compound risk (multiple threats). Score residual risk after mitigation. >15 = NO-GO, (3) model BARRIERS via Swiss Cheese (Reason) — Organizational (SMS, policies), Supervisory (dispatch, scheduling), Preconditions (MEL, crew fitness), Acts (technique, monitoring). Identify holes in each layer. Check if holes ALIGN across layers, (4) analyze HUMAN FACTORS — SHELL model (Software-Hardware-Environment-Liveware-Liveware interfaces). IMSAFE checklist. Fatigue: hours since awakening, FDP position, WOCL exposure. CRM gradient, (5) commit GO/NO-GO — binary decision. Pre-defined NO-GO criteria. "Proceed with caution" is not a decision — it is an evasion. Would you defend this on a CVR transcript read by accident investigators? If rejected, your assessment has a safety gap.

Structured reflection tool for ICAO SMS-level flight risk assessment — forces threat identification with measured parameters, risk quantification on the ICAO 5×5 matrix, Swiss Cheese barrier modeling, human factors analysis via SHELL/IMSAFE, and committed GO/NO-GO decisions. Catches Threat Blindness (generic "weather risk" instead of "CB embedded in cold front, tops FL420, movement 250°/25kt, deviation requirement 40nm right of course — adding 15 minutes and 800kg fuel burn to the trip." Every threat must have METAR/TAF data, TEM category, measurable parameters, and exposure duration), Risk Fantasy (adjective-based "medium risk" instead of ICAO 5×5 matrix scoring — "Probability C (Remote) × Severity 3 (Major) = Index 9 (Tolerable with mitigation)" is quantified. "Medium risk" is a feeling, not an assessment), Barrier Amnesia (no Swiss Cheese defense layers — Reason's model requires analysis of Organizational, Supervisory, Preconditions, and Acts layers. When holes ALIGN across all four layers, accidents happen), Human Factors Ignorance (blaming "pilot error" without SHELL model analysis — Software-Hardware-Environment-Liveware-Liveware interfaces. IMSAFE checklist. Fatigue risk: hours since sleep, FDP position, WOCL exposure), and Go-Bias (sycophantic "proceed with caution" when data demands NO-GO — "Proceed with caution" killed 346 people on two 737 MAX flights. GO or NO-GO. Binary. CVR-defensible). Call once per flight risk assessment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flight Risk Assessment Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Assess the flight risk for a B737-800 flight from EDDM to EGLL. Current METAR: EGLL 261450Z 24018G32KT 4000 +RA FEW020CB BKN035 14/11 Q1008. TAF shows CB activity until 1800Z. MEL item: weather radar degraded to 60nm range. Crew: PIC 7,500hrs (1,200 on type), FO 1,800hrs (400 on type). PIC has been awake for 14 hours. FDP at landing will be 10.5hrs of 13hr limit. Approach: ILS CAT I RWY 27L, DA 200ft. Crosswind component: 26kt (limit 33kt wet)."

**🤖 AI Agent:**
> RISK_ELEVATED — Compound risk identified: CB activity + degraded radar + PIC fatigue (14h awake). ICAO 5×5: weather C3 + radar D2 + fatigue C3. Compound index >15 = Intolerable. Recommendation: NO-GO until CB clears or crew rest.

---

**👤 You:**
> "Risk assessment for an ATR 72-600 approaching LFLB (Chambéry) at night. METAR: LFLB 261930Z 18008KT 6000 -SN SCT018 OVC025 M01/M04 Q1022. Mountains up to 12,000ft within 10nm. RNAV RWY 18 non-precision approach, MDA 3,200ft. No precision approach available. FO: 900hrs, first time at this airport. PIC reports slight headache."

**🤖 AI Agent:**
> Multiple barriers compromised: night mountain approach + non-precision + inexperienced FO + PIC health concern (IMSAFE violation). Swiss Cheese alignment detected across 3 layers. Verdict: NO-GO — crew composition inadequate for night non-precision mountain approach.

---

**👤 You:**
> "Assess compound risk: A320neo, LEMD to LPPT. MEL items: (1) APU inoperative, (2) one pack inoperative (single-pack dispatch), (3) autobrake inoperative. Departure METAR: LEMD 261600Z VRB03KT 0800 FG VV002 — fog, RVR 800m. Destination weather clear. Crew: PIC 11,000hrs, FDP 5hrs. Score each MEL item individually, then score compound risk."

**🤖 AI Agent:**
> Individual MEL items within limits. Compound risk of 3 simultaneous deferrals + low-visibility departure: cross-check dispatch minima (single-pack may restrict altitude), verify autobrake MEL dispatch conditions vs wet runway, confirm APU-off start procedure. Compound index approaches Intolerable threshold.


## ❓ FAQ

**Q: What makes this different from a standard flight risk assessment tool?**
Standard tools accept 'medium risk' as an answer. This Prover rejects anything that is not quantified on the ICAO 5×5 matrix with probability (A-E) and severity (1-5). It catches 5 specific failure modes: generic threats without METAR data, adjective-based risk without numerical scoring, missing Swiss Cheese barrier analysis, human factors reduced to 'pilot error' instead of SHELL/IMSAFE, and sycophantic go-bias where the AI says 'proceed with caution' instead of committing NO-GO when the data demands it.

**Q: How does the go-bias detection work?**
The engine maintains a semantic trap list of go-bias phrases: 'proceed with caution,' 'acceptable to proceed,' 'can proceed,' 'within acceptable limits.' If the LLM uses any of these instead of an explicit GO or NO-GO decision with pre-defined criteria, the assessment is rejected with GO_BIAS verdict. The LLM must define NO-GO criteria BEFORE the assessment and then commit to a binary decision defensible on a CVR transcript.

**Q: What aviation frameworks does this enforce?**
Five industry-standard frameworks: (1) ICAO Annex 19 Safety Management System — proactive hazard identification and risk assessment. (2) ICAO 5×5 Risk Matrix — probability × severity quantification. (3) Reason's Swiss Cheese Model — multi-layer defense analysis with hole alignment detection. (4) SHELL Model — Software-Hardware-Environment-Liveware interaction analysis for human factors. (5) Threat and Error Management (TEM) — threat categorization into environmental, airline, and crew factors per FAA AC 120-92B.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flight-risk-assessment-prover](https://vinkius.com/mcp/flight-risk-assessment-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flight Risk Assessment Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flight-risk-assessment-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flight Risk Assessment Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flight-risk-assessment-prover": {
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
