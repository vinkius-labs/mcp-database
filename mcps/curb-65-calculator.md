# CURB-65 Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/curb-65-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculate the CURB-65 score to assess pneumonia severity and treatment needs.

## Description
The CURB-65 calculator is a clinical decision support tool designed to evaluate the severity of Community-Acquired Pneumonia (CAP). By analyzing five key clinical indicators--Confusion, Urea/BUN, Respiratory Rate, Blood Pressure, and Age--it computes a total score that helps healthcare professionals determine the appropriate care setting. Use `calculate_curb65_score` to compute the score from vital signs, `get_clinical_recommendation` to interpret mortality risk and treatment settings, and `get_clinical_reference_guide` for parameter definitions.


## Available Tools (3)
- **calculate_curb65_score**: Calculate the CURB-65 score
- **get_clinical_recommendation**: Get clinical recommendation based on score
- **get_clinical_reference_guide**: Get clinical reference guide


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CURB-65 Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the CURB-65 score for a patient who is 70 years old, has a respiratory rate of 32, urea level of 25 mg/dL, systolic blood pressure of 85 mmHg, diastolic blood pressure of 55 mmHg, and is experiencing confusion."

**🤖 AI Agent:**
> The calculated CURB-65 score is 5. The criteria met include Confusion, Urea/BUN, Respiratory Rate, Blood Pressure, and Age.

---

**👤 You:**
> "What is the clinical recommendation for a CURB-65 score of 1?"

**🤖 AI Agent:**
> For a score of 1, the expected mortality risk is low, and the recommended treatment setting is outpatient care.

---

**👤 You:**
> "What does the 'Urea' parameter in CURB-65 represent?"

**🤖 AI Agent:**
> The Urea/BUN parameter refers to the Blood Urea Nitrogen level. A point is assigned if the level is greater than 19 mg/dL.


## ❓ FAQ

**Q: What is the CURB-65 score?**
The CURB-65 score is a clinical prediction rule used to assess the severity of pneumonia and estimate the risk of mortality in patients.

**Q: How do I use the calculator?**
You can provide patient vitals like respiratory rate and blood pressure to the `calculate_curb65_score` tool, then use the resulting score with `get_clinical_recommendation` to find the recommended treatment setting.

**Q: What parameters are evaluated?**
The tool evaluates Confusion, Urea/BUN levels, Respiratory Rate, Blood Pressure (systolic and diastolic), and Patient Age.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/curb-65-calculator](https://vinkius.com/mcp/curb-65-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CURB-65 Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `curb-65-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CURB-65 Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "curb-65-calculator": {
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
