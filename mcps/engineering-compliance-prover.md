# Engineering Compliance Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/engineering-compliance-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Forces AI to validate structural designs against US codes (ASCE, ACI, NEC). Demands real capacity-demand ratios, traced load paths, specific material tolerances, and FMEA instead of vague appeals to 'industry standards'.

## Description
AI agents propose engineering designs that look plausible but fail fundamentally on safety factors, load paths, and code compliance. They rely on vague appeals to 'industry standards' rather than calculating specific capacity-demand ratios or tracing loads through a system. In engineering, 'looks sturdy' is not a metric.

### The Problem It Solves

AI-generated engineering reasoning fails for five specific reasons:

- **Code blindness** — Vague references to "best practices" without citing specific normative codes (e.g., ASCE 7-22).
- **Ignored failure modes** — Prescribing a solution without analyzing HOW it could fail (yielding, buckling, fatigue) and identifying the controlling condition.
- **Ungrounded safety factors** — Failing to calculate explicit capacity-demand ratios or factors of safety.
- **Broken load paths** — Missing load assumptions (dead, live, seismic) or failure to trace forces through the structure.
- **Omitted tolerances** — Ignoring material grades, specifications, and environmental constraints. 'Steel' is not a spec.

### How It Works

Engineering Compliance Prover uses 5 Decision Pivots grounded in US engineering practice:

1. **codeComplianceValidated** — Is the design explicitly validated against a stated, specific normative code?
2. **failureModesAnalyzed** — Are the critical failure modes explicitly analyzed, identifying which one controls?
3. **safetyFactorsChecked** — Are capacity-demand ratios or factors of safety explicitly calculated and confirmed?
4. **loadPathsTraced** — Are all load assumptions explicitly stated and their path traced?
5. **tolerancesSpecified** — Are specific material grades, tolerances, and environmental conditions addressed?


## Available Tools (1)
- **validate_engineering_compliance**: Engineering is not opinion — it is code compliance, failure analysis, and proven safety margins. Lives depend on this rigor. You must: (1) define PROJECT SCOPE — system boundaries, design intent, applicable loading conditions, (2) cite the APPLICABLE CODE — exact standard with version, year, and section. "AISC 360-16, Section F2 — Flexural Members" is a code reference. "Industry standards" is rejected. Name the code or do not design, (3) detail LOAD ASSUMPTIONS — dead, live, wind, seismic, thermal, special loads. Quantified values (50 psf, 115 mph, Category C exposure). Load combinations per ASCE 7-22 Section 2.3 (LRFD or ASD), (4) analyze FAILURE MODES — FMEA methodology. Which modes are possible? Flexural yielding, lateral-torsional buckling, web crippling, connection shear, voltage drop, thermal runaway, fatigue. Which mode CONTROLS the design? How is the controlling mode mitigated?, (5) verify SAFETY FACTORS — calculate capacity-demand ratios, φRn ≥ Ru (LRFD) or Rn/Ω ≥ Ra (ASD). Show actual numbers compared to code minimums, (6) specify MATERIALS — exact grades (ASTM A992, f'c = 4000 psi), exposure classes, environmental constraints, corrosion protection, fire ratings, (7) propose DESIGN CONCLUSION — specific dimensions, sizes, ratings, parameters. Not "adequate" — the exact specification. If rejected, your engineering analysis has a structural deficiency that must be resolved.

Structured reflection tool for US engineering compliance — forces rigorous code-based analysis grounded in ASCE, ACI, AISC, NEC, and ASME standards before any design conclusion. Catches Code Compliance Blindness (referencing "industry standards" or "best practices" instead of citing a specific code section — "AISC 360-16 Section F2" is a code reference. "Industry standards for steel design" is hand-waving. Codes exist because people died), Failure Mode Ignorance (designing without analyzing how the system fails — which failure mode CONTROLS the design? Flexural yielding, lateral-torsional buckling, connection shear, voltage drop, thermal runaway? If you have not identified the controlling failure mode, you have not designed — you have guessed), Safety Factor Ungrounded ("adequate safety factor" without showing the calculation — LRFD φ factors, ASD Ω factors, capacity-demand ratios with actual numbers. The code specifies minimums. Show the math proving you exceed them), Load Path Broken (loads assumed without tracing their path through the structure — gravity, live, wind, seismic, thermal. Load combinations per ASCE 7-22 Section 2.3. A load that reaches the foundation without a traceable path is a load that finds its own path — usually through a failure), and Tolerance Omitted ("steel" without specifying ASTM A992 Fy=50 ksi, "concrete" without specifying 4000 psi f'c with exposure class — the material grade IS the design). Call once per engineering design or compliance assessment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Engineering Compliance Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We need to build a concrete retaining wall 10ft high. Ensure it's built to industry standards and is very safe against tipping over. Provide the design."

**🤖 AI Agent:**
> Verdict: CODE_COMPLIANCE_BLIND. You cite 'industry standards' and claim it will be 'very safe'. That is not an engineering specification. Name the specific code (e.g., ACI 318, ASCE 7), quantify the soil loads, calculate the factor of safety against overturning, and specify the concrete grade.

---

**👤 You:**
> "Design a W-shape steel beam spanning 20ft to support a 50 psf live load and 20 psf dead load. Validate the reasoning using the engineering compliance prover, citing AISC 360-16, checking lateral-torsional buckling, specifying ASTM A992 steel, and providing the max capacity ratio."

**🤖 AI Agent:**
> Verdict: REASONING_PROVEN. Code compliance validated (AISC 360-16), failure modes analyzed (lateral-torsional buckling checked), load paths traced (dead and live loads quantified), safety factors checked (max capacity ratio provided), and tolerances specified (ASTM A992).

---

**👤 You:**
> "Specify a 10 AWG copper wire for a 30A circuit at 100ft. Validate the code compliance against NEC, but do not analyze voltage drop or thermal limits."

**🤖 AI Agent:**
> Verdict: FAILURE_MODE_IGNORED. You validated against NEC, but intentionally ignored voltage drop and thermal runaway analysis. Name the failure mode and demonstrate that the design mitigates it.


## ❓ FAQ

**Q: Can this MCP run FEA simulations or structural math?**
No. This is a strictly stateless reasoning gatekeeper. It does not perform mathematical structural analysis or run simulations. It validates the structural logic of the AI's engineering reasoning based on the inputs provided, ensuring no assumptions are skipped.

**Q: Why did the Prover reject my design with CODE_COMPLIANCE_BLIND?**
Because the reasoning relied on vague appeals like 'industry standards' or 'standard engineering practice'. To pass the Prover, you must cite specific US codes (e.g., ASCE 7-22, AISC 360-16) and applicable sections.

**Q: What happens if I omit material grades?**
The Prover will reject the design with TOLERANCE_OMITTED. In engineering, 'steel' or 'concrete' is not a specification. You must specify exact grades like 'ASTM A992' or '4000 psi compressive strength'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/engineering-compliance-prover](https://vinkius.com/mcp/engineering-compliance-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Engineering Compliance Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `engineering-compliance-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Engineering Compliance Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "engineering-compliance-prover": {
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
