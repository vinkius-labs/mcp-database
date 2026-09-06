# Infrastructure Capex Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/infrastructure-capex-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Analyze maintenance vs growth capex and infrastructure lifecycle health.

## Description
This MCP server provides tools to evaluate the efficiency and sustainability of infrastructure spending. It allows AI agents to calculate the maintenance capex ratio, predict future growth capacity, and identify urgent asset replacement needs. By using `calculate_maintenance_ratio`, you can determine how much capital is consumed by maintenance versus expansion. Use `analyze_lifecycle_health` to assess risk levels based on asset age profiles, or `get_asset_replacement_urgency` to pinpoint which asset groups require immediate investment.


## Available Tools (4)
- **forecast_growth_capacity**: Predicts future ability to invest in growth given current depreciation and maintenance trends
- **analyze_lifecycle_health**: Evaluates the current state of the infrastructure based on how old the assets are
- **calculate_maintenance_ratio**: Determines the proportion of capital being spent on maintaining current assets versus expanding
- **get_asset_replacement_urgency**: Identifies which asset groups require immediate capital for replacement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Infrastructure Capex Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current maintenance capex ratio if maintenance is $50k, growth is $30k, and revenue is $200k?"

**🤖 AI Agent:**
> The maintenance capex ratio is 62.5%.

---

**👤 You:**
> "Which assets are most urgent to replace if our average age for critical infrastructure is 9 years and the replacement cycle is 10 years?"

**🤖 AI Agent:**
> Critical Infrastructure is identified as a priority asset due to being in the end-of-life stage.

---

**👤 You:**
> "Forecast our growth capacity with $40k maintenance, $10k depreciation, and 5% revenue growth."

**🤖 AI Agent:**
> The projected growth capacity is $10,000 with a sustainability score of 75.


## ❓ FAQ

**Q: How do I calculate the maintenance ratio?**
You can use the `calculate_maintenance_ratio` tool by providing the maintenance capex, growth capex, and total revenue.

**Q: Can I identify assets that need replacement?**
Yes, the `get_asset_replacement_urgency` tool identifies priority assets nearing the end of their lifecycle.

**Q: How is infrastructure risk assessed?**
Risk is assessed via `analyze_lifecycle_health`, which evaluates asset age profiles against the standard replacement cycle.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/infrastructure-capex-analyzer](https://vinkius.com/ai-agent-connect/infrastructure-capex-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Infrastructure Capex Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `infrastructure-capex-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Infrastructure Capex Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "infrastructure-capex-analyzer": {
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
