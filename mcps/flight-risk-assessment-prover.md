# Flight Risk Assessment Prover MCP Server

A dispatch office cleared a flight into known CB activity with 'proceed with caution.' The crew never returned. Flight Risk Prover forces ICAO SMS-level threat identification with METAR data, 5×5 risk quantification, Swiss Cheese barrier modeling, SHELL/IMSAFE human factors analysis, and explicit GO/NO-GO commitment — eliminating the sycophantic go-bias that kills in aviation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/flight-risk-assessment-prover)

## Overview
**Category:** safety & compliance
**Tools Count:** 1

## Description
Flight Risk Assessment Prover enforces ICAO Safety Management System rigor across 5 axes that LLMs consistently fail:

**Axis 1 — Threat Specificity.** Generic 'weather risk' is rejected. Every threat must be named with METAR/TAF data, TEM categories (environmental, airline, crew), measurable parameters (crosswind component, RVR vs minimums, ceiling vs DA, icing level, fuel impact), and exposure duration.

**Axis 2 — Risk Quantification.** Adjective-based 'medium risk' is rejected. Each threat is scored on the ICAO 5×5 matrix: Probability (A=Extremely Improbable to E=Frequent) × Severity (1=Negligible to 5=Catastrophic). Compound risk and post-mitigation residual risk must be calculated. Index >15 is Intolerable (NO-GO).

**Axis 3 — Barrier Modeling.** 'Safety measures in place' is rejected. Swiss Cheese defense layers must be mapped: Organizational (SMS, policies) → Supervisory (dispatch, scheduling) → Preconditions (MEL items, crew fitness) → Acts (technique, monitoring). Holes identified in each layer, alignment checked across layers.

**Axis 4 — Human Factors.** 'Pilot error' is rejected. SHELL model analysis (Software-Hardware-Environment-Liveware) plus IMSAFE checklist (Illness, Medication, Stress, Alcohol, Fatigue, Eating). Fatigue quantified: hours since sleep, FDP position, WOCL exposure.

**Axis 5 — GO/NO-GO.** 'Proceed with caution' is rejected as sycophantic go-bias. Explicit GO or NO-GO with pre-defined criteria. CVR audit: 'Would I defend this decision in an investigation?'

Every lazy shortcut — generic threats, adjective risk, missing barriers, pilot blame, or go-bias — is caught by semantic traps and consistency gates before a RISK_PROVEN verdict is issued.


## Available Tools
- **validate_flight_risk**: You must think like a Safety Officer at a major airline — the person whose signature means 200 people go airborne. You must: (1) identify THREATS with measured parameters — METAR/TAF data, TEM category (environmental, airline, crew), specific values (crosswind component, RVR, ceiling vs DA/MDA), exposure duration. "Weather risk" is rejected, (2) QUANTIFY risk on the ICAO 5×5 matrix — Probability (A=Extremely Improbable to E=Frequent) × Severity (1=Negligible to 5=Catastrophic) = Risk Index. Score compound risk (multiple threats). Score residual risk after mitigation. >15 = NO-GO, (3) model BARRIERS via Swiss Cheese (Reason) — Organizational (SMS, policies), Supervisory (dispatch, scheduling), Preconditions (MEL, crew fitness), Acts (technique, monitoring). Identify holes in each layer. Check if holes ALIGN across layers, (4) analyze HUMAN FACTORS — SHELL model (Software-Hardware-Environment-Liveware-Liveware interfaces). IMSAFE checklist. Fatigue: hours since awakening, FDP position, WOCL exposure. CRM gradient, (5) commit GO/NO-GO — binary decision. Pre-defined NO-GO criteria. "Proceed with caution" is not a decision — it is an evasion. Would you defend this on a CVR transcript read by accident investigators? If rejected, your assessment has a safety gap.

Structured reflection tool for ICAO SMS-level flight risk assessment — forces threat identification with measured parameters, risk quantification on the ICAO 5×5 matrix, Swiss Cheese barrier modeling, human factors analysis via SHELL/IMSAFE, and committed GO/NO-GO decisions. Catches Threat Blindness (generic "weather risk" instead of "CB embedded in cold front, tops FL420, movement 250°/25kt, deviation requirement 40nm right of course — adding 15 minutes and 800kg fuel burn to the trip." Every threat must have METAR/TAF data, TEM category, measurable parameters, and exposure duration), Risk Fantasy (adjective-based "medium risk" instead of ICAO 5×5 matrix scoring — "Probability C (Remote) × Severity 3 (Major) = Index 9 (Tolerable with mitigation)" is quantified. "Medium risk" is a feeling, not an assessment), Barrier Amnesia (no Swiss Cheese defense layers — Reason's model requires analysis of Organizational, Supervisory, Preconditions, and Acts layers. When holes ALIGN across all four layers, accidents happen), Human Factors Ignorance (blaming "pilot error" without SHELL model analysis — Software-Hardware-Environment-Liveware-Liveware interfaces. IMSAFE checklist. Fatigue risk: hours since sleep, FDP position, WOCL exposure), and Go-Bias (sycophantic "proceed with caution" when data demands NO-GO — "Proceed with caution" killed 346 people on two 737 MAX flights. GO or NO-GO. Binary. CVR-defensible). Call once per flight risk assessment


## Installation & Usage

To install and use the **Flight Risk Assessment Prover** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flight-risk-assessment-prover](https://vinkius.com/mcp/flight-risk-assessment-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
