# TIMI Score Calculator for ACS Risk Stratification MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/timi-score-calculator-for-acs-risk-stratification)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [risk-assessment](../categories/risk-assessment.md)

Calculates a quantitative TIMI score and provides guideline-based risk stratification for acute coronary syndrome (ACS) management.

## Description
The initial presentation of Acute Coronary Syndrome (ACS), encompassing STEMI or NSTEMI, requires rapid and accurate risk assessment to guide immediate hospital care. Early diagnosis is critical because the management strategy--whether early invasive angiography or conservative observation--determines patient survival rates and recovery time.

**Problem:** Clinicians face the challenge of rapidly synthesizing complex clinical data (age, ECG changes, lab values) into a single, actionable risk score that dictates immediate treatment pathways according to ACC/AHA guidelines. Manual calculation is slow and prone to variation.

**Mechanism:** This calculator uses three interconnected tools to create a comprehensive risk profile:
1. **`calculate_timi_score`**: Takes core clinical variables (age, ECG findings, CAD history) to generate separate TIMI scores for both STEMI and NSTEMI presentations.
2. **`derive_adverse_event_risk`**: Maps the raw calculated score and age group to a hardcoded, population-based 14-day adverse event probability.
3. **`recommend_management_strategy`**: Uses the final risk category and MI type (STEMI/NSTEMI) to recommend an immediate course of action, citing guideline justification.

**Advantage:** By automating this complex scoring cascade, the tool provides instant, evidence-based recommendations--a vital bridge connecting raw patient data to high-stakes clinical decisions.


## Available Tools (3)
- **derive_adverse_event_risk**: Translate a TIMI risk score into an estimated 14-day adverse cardiac event probability
- **recommend_management_strategy**: Recommend initial clinical management strategy based on risk category and MI type per ACC/AHA guidelines
- **calculate_timi_score**: Calculate TIMI risk scores for STEMI and NSTEMI presentation criteria based on clinical variables


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TIMI Score Calculator for ACS Risk Stratification** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the TIMI score. The patient is 65 years old, has ST elevation on ECG, and a prior CAD history of yes."

**🤖 AI Agent:**
> First, use `calculate_timi_score` to get both STEMI and NSTEMI scores. Then, if the score is high risk for STEMI, pass that result to `recommend_management_strategy` along with 'STEMI' as the condition type.

---

**👤 You:**
> "What is the 14-day adverse event probability for a patient aged Adult with a TIMI score of 5?"

**🤖 AI Agent:**
> Use `derive_adverse_event_risk` with 'Adult' as the age group and 5 as the initial score. This will give you the risk category needed for the final strategic recommendation.

---

**👤 You:**
> "We have a patient with an NSTEMI, high risk, and we need to know the next steps per guidelines. The score was 6."

**🤖 AI Agent:**
> Call `recommend_management_strategy` using 'High Risk' as the category and 'NSTEMI' as the source condition. This will provide the authoritative guideline-based pathway.


## ❓ FAQ

**Q: What inputs are required to calculate the initial TIMI score?**
The `calculate_timi_score` tool requires patient age, key ECG abnormalities (`ecgFindings`), and whether the patient has a history of Coronary Artery Disease (`priorCADHistory`). Creatinine level is optional.

**Q: Does the calculated score determine the management strategy directly?**
No. First, you use `derive_adverse_event_risk` to get a probability estimate. Then, `recommend_management_strategy` takes that risk category and the MI type (STEMI/NSTEMI) to provide the final guideline recommendation.

**Q: Can I calculate scores for different types of MIs?**
Yes. The `calculate_timi_score` tool is designed to run two separate calculations, providing distinct provisional scores tailored specifically for STEMI and NSTEMI presentations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/timi-score-calculator-for-acs-risk-stratification](https://vinkius.com/mcp/timi-score-calculator-for-acs-risk-stratification)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TIMI Score Calculator for ACS Risk Stratification** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `timi-score-calculator-for-acs-risk-stratification` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TIMI Score Calculator for ACS Risk Stratification** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "timi-score-calculator-for-acs-risk-stratification": {
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
