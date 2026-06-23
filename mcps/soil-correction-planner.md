# Soil Correction Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/soil-correction-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Plan a 3-year soil amendment program for lime, gypsum, and micronutrients.

## Description
The Soil Correction Planner helps farmers transition their soil from acidic or nutrient-deficient states to optimal levels for specific crops. Using tools like `get_lime_sequence`, `get_gypsum_sequence`, and `get_micronutrient_sequence`, you can calculate precise annual dosages of lime, gypsum, and micronutrients. The system also provides financial forecasting via `calculate_total_program_cost` to manage your 3-year investment effectively.


## Available Tools (4)
- **get_gypsum_sequence**: Calculate gypsum application doses for a 3-year period
- **get_lime_sequence**: Calculate lime application doses for a 3-year period
- **get_micronutrient_sequence**: Calculate micronutrient requirements for a crop
- **calculate_total_program_cost**: Calculate the total cost of the soil correction program


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Soil Correction Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a lime sequence for pH 4.5, target saturation 70%, using No-Till."

**🤖 AI Agent:**
> The `get_lime_sequence` tool would provide a 3-year schedule of doses with a 'Surface' application method recommendation.

---

**👤 You:**
> "What are the micronutrient needs for Corn if Zinc is at 1.5?"

**🤖 AI Agent:**
> Using `get_micronutrient_sequence`, the system will identify the deficit and provide annual dosage requirements for Zinc and other necessary elements.

---

**👤 You:**
> "Estimate total cost if lime is 50/kg, gypsum is 30/kg, and I have specific doses."

**🤖 AI Agent:**
> The `calculate_total_program_cost` tool will sum the costs of all lime, gypsum, and micronutrient applications over the 3-year period.


## ❓ FAQ

**Q: How does the lime application plan work?**
The `get_lime_sequence` tool calculates annual doses based on your current pH and target base saturation, recommending either surface or incorporated application depending on your farming system.

**Q: Can I estimate the total cost of my soil program?**
Yes, by using `calculate_total_program_cost`, you can input your calculated doses and current market prices to get a cumulative 3-year cost estimate.

**Q: Does the tool support different farming systems?**
Yes, it supports both 'No-Till' and 'Conventional' systems, adjusting application methods like surface vs. incorporated lime accordingly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/soil-correction-planner](https://vinkius.com/mcp/soil-correction-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Soil Correction Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `soil-correction-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Soil Correction Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "soil-correction-planner": {
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
