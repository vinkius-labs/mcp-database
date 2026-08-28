# Lime Requirement Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/lime-requirement-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate precise limestone requirements and application costs based on soil properties.

## Description
This MCP server provides specialized tools for agricultural soil management. It allows AI agents to determine the exact amount of lime needed to reach a target pH by analyzing soil buffering capacity, including clay content, organic matter, and Cation Exchange Capacity (CEC). Users can use `calculate_lime_rate` to find the required tonnage, `estimate_liming_cost` to project financial investments, `recommend_application_timing` to plan application windows based on lime fineness, and `get_soil_classification` to understand soil types and buffering tiers.


## Available Tools (4)
- **calculate_lime_rate**: Provide current pH, target pH, buffering method (SMP or BaseSaturation), soil properties (clay, organic matter, CEC), and lime quality (CCE and fineness factor).

Determines the total amount of lime needed to reach the target pH based on soil properties
- **estimate_liming_cost**: Calculates the financial investment required for the lime application
- **recommend_application_timing**: Provides guidance on when to apply lime based on soil characteristics and lime fineness
- **get_soil_classification**: Categorizes the soil type to provide context for the lime requirement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lime Requirement Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the lime needed for a soil with pH 5.2, target pH 6.5, using the SMP method. Soil has 25% clay, 3% organic matter, and 15 CEC. Lime has 80% CCE and 0.9 fineness."

**🤖 AI Agent:**
> The required lime rate is 4.25 tonnes per hectare.

---

**👤 You:**
> "What is the cost to apply 5 tonnes of lime if the price is $150 per tonne and application costs $30 per hectare?"

**🤖 AI Agent:**
> The total cost for the lime application is $750.00.

---

**👤 You:**
> "Classify a soil with 40% clay and 5% organic matter."

**🤖 AI Agent:**
> The soil is classified as Clay-heavy with a High Resistance buffering tier.


## ❓ FAQ

**Q: How does the tool account for lime quality?**
The `calculate_lime_rate` tool uses the Calcium Carbonate Equivalent (CCE) and the fineness factor to adjust the total lime requirement, ensuring the calculation reflects the actual effectiveness of the material.

**Q: Can I estimate the total cost of my soil treatment?**
Yes, you can use the `estimate_liming_cost` tool. By providing the lime rate and the unit price, the tool calculates both the material cost and the total investment including application costs.

**Q: What soil properties are required for the calculation?**
To get an accurate result from `calculate_lime_rate`, you need to provide the current pH, target pH, the buffering method (SMP or BaseSaturation), and soil properties including clay content, organic matter, and CEC.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/lime-requirement-calculator](https://vinkius.com/ai-agent-connect/lime-requirement-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lime Requirement Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lime-requirement-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lime Requirement Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lime-requirement-calculator": {
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
