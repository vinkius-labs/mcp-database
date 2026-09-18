# Cholesterol Risk Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cholesterol-risk-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Estimates 10-year cardiovascular risk and provides LDL targets.

## Description
This MCP server provides clinical tools to estimate cardiovascular risk using the ASCVD algorithm. It allows agents to calculate 10-year risk percentages, determine target LDL levels, evaluate risk enhancers like family history, and generate treatment guidance based on lipid profiles and patient demographics. Use `calculate_ascvd_risk` to get the baseline risk and `get_ldl_targets` to find recommended cholesterol goals.


## Available Tools (4)
- **calculate_ascvd_risk**: Calculates the primary 10-year cardiovascular risk percentage and risk category
- **evaluate_risk_enhancers**: Analyzes secondary factors that may elevate a patient's risk beyond the baseline ASCVD score
- **generate_treatment_guidance**: Provides high-level clinical considerations for medical discussion
- **get_ldl_targets**: Determines the recommended LDL cholesterol target for a specific patient


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cholesterol Risk Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the ASCVD risk for a 55-year-old male with total cholesterol 200, HDL 50, LDL 120, triglycerides 150, and systolic blood pressure 130."

**🤖 AI Agent:**
> The estimated 10-year ASCVD risk is 5.2%, which falls into the Borderline risk category.

---

**👤 You:**
> "What is the target LDL for a patient with a 15% ASCVD risk and diabetes?"

**🤖 AI Agent:**
> For a patient with a 15% risk and diabetes, the recommended target LDL is below 70 mg/dL.

---

**👤 You:**
> "Provide treatment guidance for a patient with 12% risk and a target LDL of 70."

**🤖 AI Agent:**
> Based on a 12% risk, primary recommendations include lifestyle modifications and discussing statin therapy with a physician to reach the target LDL of 70 mg/dL.


## ❓ FAQ

**Q: What is ASCVD risk?**
ASCVD risk is the estimated probability of a major cardiovascular event, such as a heart attack or stroke, occurring within the next ten years.

**Q: How can I find the target LDL level?**
You can use the `get_ldl_targets` tool after calculating the initial risk to determine the recommended LDL goal for a patient.

**Q: Does this tool account for family history?**
Yes, the `evaluate_risk_enhancers` tool specifically analyzes how family history and diabetes impact the overall clinical risk.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cholesterol-risk-calculator](https://vinkius.com/en/ai-agent-connect/cholesterol-risk-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cholesterol Risk Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cholesterol-risk-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cholesterol Risk Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cholesterol-risk-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
