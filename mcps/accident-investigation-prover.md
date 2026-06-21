# Accident Investigation Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/accident-investigation-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [safety & compliance](../categories/safety-compliance.md)

An investigation report concluded 'pilot error' and recommended 'improve training.' The same airline had three more accidents in 18 months. Accident Investigation Prover forces ICAO Annex 13 methodology — FDR/CVR evidence chains, multi-causal analysis via Reason's Model, HFACS 4-level taxonomy, organizational factor tracing, and specific, measurable, addressed recommendations that prevent recurrence.

## Description
Accident Investigation Prover enforces NTSB/ICAO Annex 13 investigation rigor across 5 axes that LLMs consistently fail:

**Axis 1 — Evidence Chain.** Narrative-based 'it appears that' is rejected. Every conclusion must be supported by FDR parameters (88 minimum per ICAO Annex 6), CVR transcript with timestamps, ATC recordings correlated with radar track, maintenance logs (MEL items, AD compliance, component life limits), and wreckage analysis (fracture type: fatigue vs overload).

**Axis 2 — Causal Chain.** Single-cause 'the accident was caused by pilot error' is rejected. NTSB format: 'The probable cause was [X], contributing to which were [Y, Z, W].' Reason's Model: latent conditions + active failures + inadequate defenses. 5-Whys to trace systemic root causes.

**Axis 3 — HFACS Taxonomy.** Unclassified 'human error' is rejected. Every factor must be classified across 4 levels: Level 1 (Unsafe Acts — errors and violations), Level 2 (Preconditions — environment, individual condition, CRM), Level 3 (Unsafe Supervision — inadequate, planned inappropriate, failed to correct), Level 4 (Organizational — resources, climate, process). If all factors cluster at Level 1, the investigation is not deep enough.

**Axis 4 — Organizational Factors.** 'The pilot should have' is rejected. Scheduling pressure (utilization rates, FDP violations), training adequacy (budget, syllabus coverage), maintenance economics (MEL deferral rates), regulatory environment (audit frequency), and financial pressure are mandatory analysis targets.

**Axis 5 — Recommendation Actionability.** 'Improve training' is rejected. Every recommendation must be: Specific (what action), Measurable (success criteria), Addressed (to named authority), Tracked (follow-up timeline), Evidence-linked (to which finding).

ICAO Annex 13, 3.1: 'The sole objective shall be the prevention of accidents. It is NOT the purpose to apportion blame or liability.'


## Available Tools (1)
- **validate_accident_investigation**: Before reaching any investigation conclusion, call this tool. You must: (1) CORRELATE EVIDENCE — FDR 88 parameters with timestamps, CVR transcript correlation, ATC radar track and clearances, maintenance logs (MEL, AD compliance, component TSN/TSO), wreckage analysis (fracture type: fatigue vs overload, fire pattern, impact signatures). Cross-reference ALL sources — narrative without data is speculation, (2) CONSTRUCT CAUSAL CHAIN — probable cause + contributing factors (NTSB format: "Probable cause was [X], contributing to which were [Y, Z, W]"). Apply 5-Whys to reach systemic causes. Map to Reason's Model: latent conditions + active failures + defense gaps, (3) CLASSIFY via HFACS — every factor at its correct level: Level 1 (unsafe acts: decision/skill/perceptual errors, routine/exceptional violations), Level 2 (preconditions: environment, individual condition, CRM), Level 3 (supervision: inadequate, planned inappropriate, failed to correct, supervisory violations), Level 4 (organizational: resources, climate, process). If all factors cluster at Level 1, you have not investigated deeply enough, (4) ANALYZE ORGANIZATIONAL factors — scheduling pressure, training budget, maintenance economics, regulatory oversight gaps, financial pressure on safety decisions. The pilot is the LAST link in a chain that starts with organizational decisions months or years before, (5) WRITE ACTIONABLE RECOMMENDATIONS — specific (what action), measurable (success criteria), addressed (to named authority), tracked (response timeline + verification), evidence-linked (to which finding). "Improve training" is a wish — not a recommendation. If rejected, your investigation has a structural deficiency — deepen the analysis.

Structured reflection tool for ICAO Annex 13/NTSB-standard accident investigation. Forces the agent to construct multi-causal, evidence-correlated, taxonomy-classified investigation analyses before reaching any conclusion. Catches Evidence Gaps (narrative without FDR/CVR cross-reference), Single Cause Fallacy (blaming one factor instead of Reason's Swiss Cheese Model), HFACS Blindness (labeling "human error" without 4-level taxonomy classification), Organizational Amnesia (ignoring scheduling, training, maintenance, and regulatory systemic pressures), and Recommendation Theater (vague "improve training" instead of specific, measurable, addressed, tracked, evidence-linked actions). Call once per investigation analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accident Investigation Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Investigate: A B737-800 crashed 2nm short of runway during ILS approach in IMC. FDR shows airspeed decreased from 145kt to 108kt over 22 seconds with no crew action until stick shaker. CVR shows no speed callout from PM. PIC had been on duty 11.5 hours. Autothrottle deferred (MEL C) for 5 days. No unreliable airspeed training in 24 months. National authority had not audited the operator in 28 months."

**🤖 AI Agent:**
> Multi-causal analysis: probable cause — loss of airspeed awareness (Level 1) due to autothrottle deferral (Level 2/maintenance), fatigue at 11.5h FDP (Level 2/precondition), inadequate CRM monitoring (Level 3/supervision), 24-month training gap (Level 4/organizational), 28-month audit gap (Level 4/regulatory). HFACS traversal reaches Level 4. 'Pilot error' rejected as root cause.

---

**👤 You:**
> "Investigate: ATR 42-500 impacted terrain at 4,800ft during non-precision approach to a mountain airport at night. MDA was 4,200ft. FDR shows descent below MDA without missed approach. CVR: PIC said 'I have the runway' at 4,500ft — airport was 8nm away. GPWS 'TERRAIN' warning 4 seconds before impact. FO on first flight to this airport. No special airport qualification program."

**🤖 AI Agent:**
> CFIT — Controlled Flight Into Terrain. Multi-causal: visual illusion below MDA (Level 1), inadequate crew pairing for high-risk airport (Level 3), absent special airport qualification program (Level 4). GPWS response time insufficient (4s). Investigation must reach Level 4 organizational factors.

---

**👤 You:**
> "Investigate: A320 uncontained engine failure on takeoff at V1+5. LP turbine disk separated. Replacement part from third-party supplier, installed 340 flight hours ago. Traceability gap between OEM and supplier. Operator used this supplier 18 months — 23% cheaper than OEM. National authority had approved the supplier."

**🤖 AI Agent:**
> Organizational factors dominant: cost-driven supplier selection (Level 4), traceability gap in part documentation (Level 3/supervision), inadequate authority oversight of third-party suppliers (Level 4/regulatory). Recommendations must address: supplier audit frequency, traceability chain verification, OEM vs third-party risk assessment framework.


## ❓ FAQ

**Q: How does this prevent 'pilot error' as a root cause conclusion?**
The engine maintains a semantic trap list of blame-language signals: 'pilot error,' 'crew error,' 'human error,' 'judgment error,' 'failed to,' 'negligence.' If the LLM uses any of these in the HFACS taxonomy field, the classification is rejected. Instead, the LLM must classify each factor at the correct HFACS level: Level 1 (what the pilot did — skill error, decision error, perceptual error, or violation), Level 2 (what conditions enabled it — fatigue, CRM failure, environment), Level 3 (what supervision allowed it — scheduling, training gaps), Level 4 (what organizational decisions created it — budget cuts, staffing, regulatory gaps). 'Pilot error' is Level 1 only — the investigation must reach Level 4.

**Q: What evidence sources must be cross-referenced?**
Five mandatory sources: (1) Flight Data Recorder — minimum 88 parameters per ICAO Annex 6, with timestamps. (2) Cockpit Voice Recorder — last 2 hours of audio, transcribed with timestamps, correlated with FDR parameter changes. (3) ATC recordings — radar track, clearances, handoffs, weather advisories. (4) Maintenance logs — last A/B/C/D checks, MEL items, deferred defects, AD compliance, component life (TSN/TSO/CSN/CSO). (5) Wreckage analysis — impact signatures, fire patterns, fracture analysis (fatigue vs overload), metallurgical examination. The engine rejects speculative language like 'it appears that' or 'evidence suggests' when hard data from these sources exists.

**Q: Why does this require recommendations to be addressed to specific authorities?**
Because 'improve training' with no addressee has zero accountability. The NTSB model requires each recommendation to name the authority responsible for implementation — the FAA, the operator, the manufacturer, or an international body. Each recommendation must include: what specific action to take, measurable success criteria, a response deadline (typically 90 days), a verification mechanism (audit, inspection, data review), and a direct link to a specific investigation finding. This is how aviation achieved its extraordinary safety record — not through vague wishes, but through tracked, accountable, evidence-linked changes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/accident-investigation-prover](https://vinkius.com/mcp/accident-investigation-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accident Investigation Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accident-investigation-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accident Investigation Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accident-investigation-prover": {
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
