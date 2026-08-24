# HbA1c to Average Glucose Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/hba1c-to-average-glucose-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Estimate average glucose, time in range, and glucose variability from HbA1c.

## Description
This MCP server provides deterministic tools to convert HbA1c percentages into clinical glucose metrics. Using the ADAG formula, it calculates estimated average glucose (eAG) in both mg/dL and mmol/L. It also provides statistical estimates for Time in Range (TIR) and the Coefficient of Variation (CV) based on standard regression models. Use `calculate_glucose_metrics` to get a full profile of glucose metrics, `get_conversion_constants` to see the underlying math, or `validate_a1c_range` to check if a value is clinically valid.


## Available Tools (3)
- **get_conversion_constants**: Get the mathematical constants used for glucose conversions
- **calculate_glucose_metrics**: Calculate estimated glucose metrics based on HbA1c percentage
- **validate_a1c_range**: Validate if an HbA1c value is within a clinically valid range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HbA1c to Average Glucose Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Based on this HbA1c percentage, what are my estimated average glucose, time in range, and glucose variability? My HbA1c is 7.0%."

**🤖 AI Agent:**
> For an HbA1c of 7.0%, your estimated average glucose is 154 mg/dL (8.5 mmol/L), with an estimated Time in Range of approximately 70% and a Coefficient of Variation of 33%.

---

**👤 You:**
> "What are the mathematical constants used for these glucose conversions?"

**🤖 AI Agent:**
> The conversion uses a mg/dL to mmol/L factor of 18.018 and assumes a standard CV range for statistical estimations.

---

**👤 You:**
> "Is an HbA1c of 4.5% valid for estimation?"

**🤖 AI Agent:**
> Yes, an HbA1c of 4.5% is within the clinically valid range for these estimation models.


## ❓ FAQ

**Q: How is the average glucose calculated?**
The estimated average glucose (eAG) is calculated using the ADAG formula: (28.7 × HbA1c) - 46.7.

**Q: Can I validate if my HbA1c value is within a realistic range?**
Yes, you can use the `validate_a1c_range` tool to check if a specific HbA1c percentage falls within a clinically meaningful and physiologically valid range.

**Q: What metrics are provided in the full report?**
The `calculate_glucose_metrics` tool provides the HbA1c percentage, eAG in mg/dL, eAG in mmol/L, estimated Time in Range (TIR), and the estimated Coefficient of Variation (CV).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/hba1c-to-average-glucose-converter](https://vinkius.com/ai-agent-connect/hba1c-to-average-glucose-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HbA1c to Average Glucose Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hba1c-to-average-glucose-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HbA1c to Average Glucose Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hba1c-to-average-glucose-converter": {
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
