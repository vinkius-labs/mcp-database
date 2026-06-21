# Fertilizer Requirement Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fertilizer-requirement-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate precise nutrient dosages and fertilizer costs based on soil analysis and regional standards.

## Description
This MCP server provides specialized tools for agricultural planning. Use `analyze_soil_chemistry` to interpret pH, P, K, Ca, and Mg levels to determine soil fertility status. Use `compute_nutrient_demands` to calculate the required kilograms per hectare of N, P₂O₅, and K₂O based on regional standards like IAC-SP, EMBRAPA, or CFSEMG. Finally, use `generate_fertilizer_plan` to convert these nutrient requirements into a concrete application plan with specific commercial products and total cost estimates.


## Available Tools
- **analyze_soil_chemistry**: Provides a qualitative interpretation of the soil health based on chemical laboratory results
- **compute_nutrient_demands**: Calculates the specific kilograms per hectare of N, P2O5, and K2O needed to achieve a target productivity
- **generate_fertilizer_plan**: Converts nutrient requirements into physical product weights and total cost estimates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fertilizer Requirement Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this soil sample: pH 5.5, P 10, K 80, Ca 40, Mg 20."

**🤖 AI Agent:**
> The `analyze_soil_chemistry` tool would evaluate these values to determine the acidity level and fertility status of your soil.

---

**👤 You:**
> "Calculate nutrient needs for Corn with 10 tons/ha yield using EMBRAPA standards."

**🤖 AI Agent:**
> The `compute_nutrient_demands` tool will calculate the necessary N, P2O5, and K2O based on the EMBRAPA guidelines.

---

**👤 You:**
> "Generate a plan for 50kg N, 30kg P, and 40kg K using available fertilizers."

**🤖 AI Agent:**
> The `generate_fertilizer_plan` tool will identify the best products to meet these requirements and estimate the total cost.


## ❓ FAQ

**Q: What regional standards are supported?**
The server supports IAC-SP, EMBRAPA, and CFSEMG regulatory and agronomic tables.

**Q: How do I calculate the cost of fertilization?**
Use the `generate_fertilizer_plan` tool. By providing your nutrient requirements and a list of available products, it calculates the total cost per hectare.

**Q: Can I use this for different crop types?**
Yes, the `compute_nutrient_demands` tool allows you to specify various crops and their expected yields.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fertilizer-requirement-calculator](https://vinkius.com/mcp/fertilizer-requirement-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fertilizer Requirement Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `fertilizer-requirement-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fertilizer Requirement Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fertilizer-requirement-calculator": {
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
