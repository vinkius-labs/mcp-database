# Dairy Lactation Curve Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/dairy-lactation-curve-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predict dairy cow milk production trajectories using Wood's and Wilmink's mathematical models.

## Description
This MCP server provides advanced mathematical modeling for dairy herd management. It uses Wood's gamma function and Wilmink's exponential model to predict milk production patterns. Users can calculate specific daily yields with `get_daily_production`, determine total milk produced via `get_cumulative_yield`, and forecast long-term metrics like 305-day yield and persistency using `get_lactation_projections`. Additionally, `predict_economic_schedule` helps optimize dry-off dates and evaluate calving interval economics.


## Available Tools (4)
- **get_cumulative_yield**: Calculates the total volume of milk produced from calving up to a specific day
- **get_daily_production**: Determines the specific milk volume produced on a given day
- **get_lactation_projections**: Predicts long-term production metrics including 305-day yield and the persistency of the cow
- **predict_economic_schedule**: Estimates the optimal dry-off date and the resulting economic implications for the calving interval


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dairy Lactation Curve Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much milk will this cow produce on day 150 if her peak was 40kg on day 50 and she is parity 2 using the woods model?"

**🤖 AI Agent:**
> On day 150, the predicted daily milk yield is 22.45kg.

---

**👤 You:**
> "What is the projected 305-day yield for a cow with a peak of 45kg on day 40 and parity 1 using the wilmink model?"

**🤖 AI Agent:**
> The projected 305-day yield is 10,250kg.

---

**👤 You:**
> "Calculate the total milk produced up to day 200 for a cow with peak 35kg on day 45 and parity 3 using the woods model."

**🤖 AI Agent:**
> The total cumulative yield up to day 200 is 5,120kg.


## ❓ FAQ

**Q: What mathematical models are supported?**
The server supports Wood's gamma function and Wilmink's exponential model for modeling lactation curves.

**Q: How can I predict the total milk yield for a cow?**
You can use the `get_cumulative_yield` tool to calculate the total volume of milk produced from calving up to a specific day.

**Q: Can this model help with economic planning?**
Yes, the `predict_economic_schedule` tool estimates optimal dry-off dates and provides an economic impact score related to the calving interval.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/dairy-lactation-curve-model](https://vinkius.com/ai-agent-connect/dairy-lactation-curve-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dairy Lactation Curve Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dairy-lactation-curve-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dairy Lactation Curve Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dairy-lactation-curve-model": {
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
