# BMI Clinical Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bmi-clinical-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculate BMI, ideal body weight estimates, and assess bariatric surgery eligibility.

## Description
This MCP server provides clinical tools for anthropometric assessment. Use `compute_bmi_metrics` to calculate Body Mass Index (BMI) along with WHO classification and ASMBS risk categories. The `calculate_ideal_body_weights` tool estimates healthy weight using Devine, Hamwi, and Robinson formulas. Additionally, use `evaluate_bariatric_eligibility` to determine surgical candidacy based on NIH criteria.


## Available Tools (3)
- **calculate_ideal_body_weights**: Estimate ideal body weight using clinical formulas
- **compute_bmi_metrics**: Calculate BMI and related clinical metrics
- **evaluate_bariatric_eligibility**: Determine bariatric surgery eligibility


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BMI Clinical Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the BMI metrics for a person weighing 95kg and 175cm tall."

**🤖 AI Agent:**
> The calculated BMI is 31.0, which falls under the Obesity Class I category according to WHO standards. The ASMBS metabolic risk category is also identified.

---

**👤 You:**
> "What is the ideal body weight for a female who is 160cm tall?"

**🤖 AI Agent:**
> Using clinical formulas, the estimated ideal weights are: Devine: 52.2kg, Hamwi: 51.4kg, and Robinson: 50.8kg.

---

**👤 You:**
> "Is a patient with a BMI of 36 and hypertension eligible for bariatric surgery?"

**🤖 AI Agent:**
> Yes, the patient is eligible for surgery because they meet the NIH criteria of having a BMI ≥ 35 with existing comorbidities.


## ❓ FAQ

**Q: How do I calculate BMI and weight categories?**
Use the `compute_bmi_metrics` tool by providing the patient's weight in kilograms and height in centimeters.

**Q: Can I estimate ideal body weight?**
Yes, the `calculate_ideal_body_weights` tool provides estimates using the Devine, Hamwi, and Robinson formulas.

**Q: How is bariatric eligibility determined?**
The `evaluate_bariatric_eligibility` tool evaluates candidacy based on NIH criteria, considering BMI and the presence of comorbidities.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bmi-clinical-calculator](https://vinkius.com/mcp/bmi-clinical-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BMI Clinical Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bmi-clinical-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BMI Clinical Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bmi-clinical-calculator": {
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
