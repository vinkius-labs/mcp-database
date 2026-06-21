# GRACE Score Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/grace-score-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cardiology](../categories/cardiology.md)

Calculates the Global Registry of Acute Coronary Events (GRACE) risk score to predict in-hospital and six-month mortality for ACS patients.

## Description
The clinical assessment of a patient with Acute Coronary Syndrome (ACS) requires more than just looking at vital signs. A comprehensive risk score is needed to predict short-term mortality and guide immediate treatment decisions. The GRACE Score Calculator addresses this gap by providing a standardized, clinically validated toolset for accurate risk stratification.

### How it works:
The system takes nine core clinical parameters--including age, heart rate, systolic blood pressure, creatinine level, Killip class, cardiac arrest status, ST deviation, and troponin concentration. It uses these inputs to compute the composite GRACE score (0-100).

**Mechanism:**
1.  The primary calculation is handled by `calculate_grace_score`. This tool computes a weighted risk score based on established medical guidelines.
2.  Once the raw score is generated, `get_risk_category` maps that numerical output to an actionable risk category (Low, Intermediate, or High). 
3.  Furthermore, the system estimates both in-hospital and six-month mortality probabilities using hardcoded lookup tables for precise clinical prediction.

The result provides a clear, data-driven view of the patient's immediate and long-term prognosis, allowing care teams to prioritize resources and intervene before adverse events occur.


## Available Tools
- **calculate_grace_score**: Calculate GRACE risk score for acute coronary syndrome patients
- **get_risk_category**: Get risk category and recommendation for a GRACE score


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GRACE Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the GRACE score for a 65-year-old male with HR of 90, SBP of 120, creatinine of 1.1, Killip Class II, no cardiac arrest, ST deviation of 1, and troponin elevated."

**🤖 AI Agent:**
> First, I will call `calculate_grace_score` with the provided vitals. Then, using the resulting score, I will call `get_risk_category` to get the final risk assessment and mortality estimates.

---

**👤 You:**
> "I need an estimated 6-month mortality risk for a patient with a calculated GRACE score of 78, who is age 75 and Killip Class III."

**🤖 AI Agent:**
> To determine the long-term prognosis, I will use `get_risk_category` (or a related prediction endpoint if available) with the score of 78. This function is designed to provide mortality estimates based on age and Killip class.

---

**👤 You:**
> "What are the critical parameters for the calculator?"

**🤖 AI Agent:**
> The core calculation relies on inputting vitals like SBP, HR, and lab results (creatinine/troponin) via `calculate_grace_score` to generate the initial score.


## ❓ FAQ

**Q: What inputs are required for the GRACE score calculation?**
The `calculate_grace_score` tool requires nine key parameters: age, heart rate, systolic blood pressure, potassium, creatinine, Killip class, cardiac arrest status, ST deviation, and enzyme elevation. Providing accurate data for all fields is critical for an accurate score.

**Q: Does the tool provide more than just a numerical score?**
No. The system uses `get_risk_category` to translate the raw score into an actionable risk category (Low, Intermediate, High), providing immediate clinical recommendations and estimated mortality ranges for both hospital stay and six months post-discharge.

**Q: Is this tool suitable for all patients with chest pain?**
The GRACE score is designed specifically for Acute Coronary Syndrome (ACS) patients. While the `calculate_grace_score` tool can accept general vital signs, clinical interpretation must be done by a qualified medical professional.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/grace-score-calculator](https://vinkius.com/mcp/grace-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GRACE Score Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `grace-score-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GRACE Score Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grace-score-calculator": {
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
