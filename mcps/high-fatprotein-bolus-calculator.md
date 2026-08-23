# High-Fat/Protein Bolus Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/high-fatprotein-bolus-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculates insulin dosing for high-fat and high-protein meals to mitigate the 'Pizza Effect'.

## Description
This MCP server provides deterministic insulin dosing strategies for meals with significant fat and protein content. It addresses the 'Pizza Effect'--the delayed glucose rise caused by non-carbohydrate macronutrients--by calculating Fat-Protein Units (FPU) and recommending a dual-wave delivery method. Use `calculate_meal_bolus` to determine the total insulin, immediate dose, and extended dose, or `get_macronutrient_summary` to verify meal composition.


## Available Tools (3)
- **calculate_meal_bolus**: 
- **get_macronutrient_summary**: 
- **validate_icr_threshold**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **High-Fat/Protein Bolus Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the insulin dose for a meal with 60g carbs, 30g fat, and 20g protein using an ICR of 50."

**🤖 AI Agent:**
> The total insulin required is 3.0 units. This includes a standard bolus of 1.2 units and 1.8 units of FPU. The immediate dose is 1.8 units and the extended dose is 1.2 units over 2.5 hours.

---

**👤 You:**
> "I had a meal with 40g carbs, 10g fat, and 5g protein. My ICR is 40. What is my dose?"

**🤖 AI Agent:**
> The total insulin required is 1.0 unit. Since the combined fat and protein is 15g (below the 40g threshold), no FPU is added. The immediate dose is 0.6 units and the extended dose is 0.4 units.

---

**👤 You:**
> "Check if my ICR of 10 is within the safe range."

**🤖 AI Agent:**
> Yes, an ICR of 10 is within the valid physiological range.


## ❓ FAQ

**Q: What is the 'Pizza Effect'?**
The 'Pizza Effect' is the significant rise in blood glucose levels that occurs several hours after consuming meals high in fat and protein, as these macronutrients slow gastric emptying.

**Q: How does the calculator handle high-fat meals?**
When combined fat and protein exceed 40g, the `calculate_meal_bolus` tool adds Fat-Protein Units (FPU) to the standard carbohydrate dose and suggests a split-dose delivery.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/high-fatprotein-bolus-calculator](https://vinkius.com/ai-agent-connect/high-fatprotein-bolus-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **High-Fat/Protein Bolus Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `high-fatprotein-bolus-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **High-Fat/Protein Bolus Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "high-fatprotein-bolus-calculator": {
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
