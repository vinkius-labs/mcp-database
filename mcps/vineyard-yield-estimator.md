# Vineyard Yield Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/vineyard-yield-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predict grape yields and harvest timelines using phenological models.

## Description
This MCP server provides precise viticulture intelligence. It allows AI agents to calculate expected grape mass per hectare and predict harvest windows using the Baggiolini phenology model. By analyzing vine architecture, pruning methods like `CANE` or `SPUR`, and canopy density, the system provides actionable yield metrics. It also assesses vineyard health and stability to help manage production risks.


## Available Tools (3)
- **calculate_yield_metrics**: Calculate expected grape yield metrics per hectare
- **predict_harvest_date**: Predict the estimated harvest date based on phenological stages
- **get_vineyard_health_summary**: Get a summary of vineyard health and productivity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vineyard Yield Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected yield for a vineyard with 2500 vines per hectare, 40 buds per vine, and 0.8 fruitfulness?"

**🤖 AI Agent:**
> The estimated total yield for your vineyard is 12,500 kilograms per hectare.

---

**👤 You:**
> "When will the grapes be ready if they are currently in the VERAISON stage at 25 degrees Celsius?"

**🤖 AI Agent:**
> The grapes are expected to reach the MATURITY stage in approximately 14 days.

---

**👤 You:**
> "How does my canopy density affect my yield risk?"

**🤖 AI Agent:**
> With a canopy density of 0.7 and cane pruning, your productivity multiplier is 0.95 and the risk level is Low.


## ❓ FAQ

**Q: How does the tool calculate yield?**
The `calculate_yield_metrics` tool uses vine density, bud count, fruitfulness, and berry weight to determine the total expected mass per hectare.

**Q: Can I predict the harvest date?**
Yes, by using `predict_harvest_date`, you can estimate the days remaining until harvest based on the current Baggiolini stage and temperature.

**Q: What pruning methods are supported?**
The system supports `SPUR`, `CANE`, and `MECHANICAL` pruning methods to adjust yield expectations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/vineyard-yield-estimator](https://vinkius.com/ai-agent-connect/vineyard-yield-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vineyard Yield Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vineyard-yield-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vineyard Yield Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vineyard-yield-estimator": {
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
