# HAS-BLED Score Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/has-bled-score-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Assess major bleeding risk in patients on anticoagulation therapy using the HAS-BLED scoring system.

## Description
The HAS-BLED Score Calculator is a clinical decision support tool designed to identify patients at high risk of major bleeding while receiving oral anticoagulants. By evaluating seven key clinical indicators--Hypertension, Abnormal Coagulation, Stroke history, Bleeding history, Labile INR, Elderly status (65+), and use of Drugs or Alcohol--the tool provides a quantitative score. Use the `calculate_has_ble_score` tool to compute the integer score, `get_risk_interpretation` to understand the qualitative risk level and management recommendations, and `get_scoring_criteria_reference` to review the clinical definitions for each scoring factor.


## Available Tools (3)
- **calculate_has_ble_score**: Compute the quantitative HAS-BLED integer score
- **get_risk_interpretation**: Translate a numerical HAS-BLED score into a qualitative risk category
- **get_scoring_criteria_reference**: Provide a descriptive reference for all potential scoring variables


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HAS-BLED Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the HAS-BLED score for a 70-year-old patient with hypertension, a history of stroke, and recent use of NSAIDs."

**🤖 AI Agent:**
> The calculated HAS-BLED score is 3, indicating a high risk of major bleeding.

---

**👤 You:**
> "What are the clinical management recommendations for a patient with a HAS-BLED score of 1?"

**🤖 AI Agent:**
> A score of 1 indicates low risk, suggesting continuation of anticoagulation therapy with routine monitoring as per standard guidelines.

---

**👤 You:**
> "Show me the criteria used for the HAS-BLED score calculation."

**🤖 AI Agent:**
> The scoring factors include hypertension (systolic > 160 mmHg), abnormal coagulation, stroke history, bleeding history, labile INR, elderly status (≥65), and drugs/alcohol use.


## ❓ FAQ

**Q: What is the HAS-BLED score used for?**
It is a clinical scoring system used to identify patients at high risk of major bleeding when using oral anticoagulants like Warfarin or DOACs.

**Q: How do I interpret a high score?**
A score of 3 or higher indicates a high risk of bleeding, necessitating intensified clinical monitoring and careful evaluation of reversible risk factors.

**Q: Which clinical indicators are included in the calculation?**
The score includes hypertension, abnormal coagulation (renal/hepatic), stroke history, bleeding history, labile INR, age (65+), and use of drugs or alcohol.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/has-bled-score-calculator](https://vinkius.com/mcp/has-bled-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HAS-BLED Score Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `has-bled-score-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HAS-BLED Score Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "has-bled-score-calculator": {
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
