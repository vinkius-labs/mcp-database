# Pediatric Fluid Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pediatric-fluid-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculate pediatric fluid maintenance requirements using the Holliday-Segar rule.

## Description
This MCP server provides precise clinical calculations for determining pediatric fluid maintenance needs based on the Holliday-Segar method. It allows healthcare professionals to calculate `calculate_daily_volume`, determine the `calculate_hourly_rate`, and retrieve `get_electrolyte_recommendation` based on a patient's weight in kilograms. The tool handles weight segments automatically: 4ml/kg for the first 10kg, 2ml/flag for the next 10kg, and 1ml/kg for any mass above 20kg.


## Available Tools (3)
- **get_electrolyte_recommendation**: Get electrolyte concentration recommendations
- **calculate_daily_volume**: Returns total ml per 24h and distribution details.

Calculate total daily fluid volume using Holliday-Segar rule
- **calculate_hourly_rate**: Returns ml per hour.

Calculate hourly fluid infusion rate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pediatric Fluid Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the daily fluid volume for a child weighing 15kg."

**🤖 AI Agent:**
> For a weight of 15kg, the total daily volume is 80ml/day. This includes 40ml for the first 10kg and 20ml for the next 5kg.

---

**👤 You:**
> "What is the hourly infusion rate for a 25kg patient?"

**🤖 AI Agent:**
> The required hourly infusion rate for a 25kg patient is 104.17 ml/hour.

---

**👤 You:**
> "What are the electrolyte recommendations for an 8kg infant?"

**🤖 AI Agent:**
> For an 8kg patient (Neonatal/Infant Tier), the recommended concentration is 150 mEq/L of Sodium and 75 mEq/L of Potassium.


## ❓ FAQ

**Q: What is the Holliday-Segar rule?**
The Holliday-Segar rule is a standard clinical method used to estimate daily fluid requirements for pediatric patients by applying different fluid densities to specific weight segments.

**Q: How do I use the `calculate_daily_volume` tool?**
Provide the patient's weight in kilograms as input. The tool will return the total volume required for a 24-hour period and a summary of how that volume was distributed across weight tiers.

**Q: Can this tool recommend electrolyte concentrations?**
Yes, by using the `get_electrolyte_recommendation` tool with the patient's weight, you can find the recommended milliequivalents of Sodium and Potassium per liter for their specific clinical tier.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pediatric-fluid-calculator](https://vinkius.com/mcp/pediatric-fluid-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pediatric Fluid Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pediatric-fluid-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pediatric Fluid Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pediatric-fluid-calculator": {
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
