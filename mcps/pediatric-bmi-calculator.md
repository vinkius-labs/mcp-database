# Pediatric BMI Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pediatric-bmi-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate pediatric BMI, percentiles, and growth status using WHO/CDC standards for ages 2-20 years.

## Description
This MCP server provides a specialized calculation engine for assessing pediatric BMI, percentiles, and growth status. Using hardcoded WHO (World Health Organization) and CDC (Centers for Disease Dynamics) reference tables, it maps BMI values to specific percentiles and z-scores for children aged 2 to 20 years. You can use `calculate_bmi` to compute the index, `assess_growth_metrics` to determine nutritional classification, and `validate_pediatric_parameters` to ensure all biological data is within valid clinical bounds.


## Available Tools (3)
- **calculate_bmi**: Calculate BMI index
- **assess_growth_metrics**: Assess pediatric growth metrics
- **validate_pediatric_parameters**: Validate pediatric parameters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pediatric BMI Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the BMI for a 5-year-old boy weighing 20kg and 110cm tall."

**🤖 AI Agent:**
> The calculated BMI is 16.53. For a 60-month-old male, this falls within the healthy weight range.

---

**👤 You:**
> "Is a BMI of 25 for a 14-year-old female considered overweight?"

**🤖 AI Agent:**
> A BMI of 25 for a 168-month-old female corresponds to the overweight classification based on CDC growth charts.

---

**👤 You:**
> "Check if these parameters are valid: age 12 months, weight 5kg."

**🤖 AI Agent:**
> The parameters are invalid. The supported age range for pediatric assessment is between 24 and 240 months.


## ❓ FAQ

**Q: What age range is supported?**
The calculator supports children and adolescents between 24 and 240 months (2 to 20 years) of age.

**Q: Which growth standards are used?**
The engine uses hardcoded WHO and CDC reference tables to ensure accurate percentile and z-score calculations.

**Q: How do I calculate the BMI index?**
Use the `calculate_bmi` tool by providing the weight in kilograms and height in centimeters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pediatric-bmi-calculator](https://vinkius.com/mcp/pediatric-bmi-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pediatric BMI Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pediatric-bmi-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pediatric BMI Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pediatric-bmi-calculator": {
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
