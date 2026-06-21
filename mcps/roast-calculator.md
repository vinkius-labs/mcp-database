# Roast Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/roast-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [culinary](../categories/culinary.md)

Precise cooking time, resting duration, and carryover temperature predictions for meat roasting.

## Description
The Roast Calculator MCP server provides specialized culinary computations for professional and home roasting. By connecting AI agents to precise thermal models, it enables accurate predictions of cooking duration using `calculate_cooking_duration`, recommended resting periods via `calculate_rest_duration`, and temperature shifts during the rest phase with `estimate_carrylag_impact`.


## Available Tools (3)
- **estimate_carryover_impact**: Estimate the temperature increase due to carryover cooking
- **calculate_cooking_duration**: Calculate the estimated total cooking time for a roast
- **calculate_rest_duration**: Calculate the recommended resting time for a roast


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Roast Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long will a 2kg Beef roast take at 150C?"

**🤖 AI Agent:**
> You should use the `calculate_cooking_duration` tool with meatType: 'Beef', weightKg: 2, and ovenTemperatureCelsius: 150 to get the exact estimate.

---

**👤 You:**
> "How much will the temperature rise for a Pork roast?"

**🤖 AI Agent:**
> To find this, use `estimate_carryover_impact` with your removal and target temperatures.

---

**👤 You:**
> "What is the resting time for a 5kg roast?"

**🤖 AI Agent:**
> Use `calculate_rest_duration` with weightKg: 5 to determine the optimal rest period.


## ❓ FAQ

**Q: How can I calculate how long my beef roast will take?**
You can use the `calculate_cooking_duration` tool by providing the meat type (Beef), weight in kg, and your target oven temperature.

**Q: Does this tool help with resting time?**
Yes. The `calculate_rest_duration` tool estimates the necessary rest period based on the thermal mass of your roast.

**Q: Can I predict temperature changes after taking meat out of the oven?**
Yes, use `estimate_carryover_impact` to predict the internal temperature rise during the resting phase.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/roast-calculator](https://vinkius.com/mcp/roast-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Roast Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `roast-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Roast Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "roast-calculator": {
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
