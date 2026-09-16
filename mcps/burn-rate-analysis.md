# Burn Rate Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/burn-rate-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze startup burn rates, trends, and projected runway.

## Description
This MCP server provides essential financial intelligence for startups. It allows AI agents to calculate gross and net burn, evaluate burn trends, detect financial anomalies, and project the runway zero date. Use `get_current_burn_metrics` for immediate monthly status, `analyze_burn_trends` to understand cash consumption trajectory, `project_runway` to estimate remaining months of cash, and `identify_anomalies` to isolate one-time expenses that skew data.


## Available Tools (4)
- **get_current_burn_metrics**: Calculates the immediate financial status for a specific month
- **analyze_burn_trends**: Evaluates the trajectory of cash consumption over a provided period
- **identify_anomalies**: Detects one-time expenses or revenue spikes that distort the true burn rate
- **project_runway**: Predicts the "Zero Date" (when cash runs out) based on current cash and historical burn


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Burn Rate Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current financial status for last month with $50,000 expenses and $20,000 revenue?"

**🤖 AI Agent:**
> Your gross burn was $50,000 and your net burn was $30,000. Your current status is burning.

---

**👤 You:**
> "Based on $100,000 cash and a net burn history of [10000, 12000, 11000], how much runway do we have left?"

**🤖 AI Agent:**
> You have approximately 8.7 months of runway remaining.

---

**👤 You:**
> "Analyze our burn trend with expenses [10, 12, 15, 11] and revenue [2, 3, 4, 3]."

**🤖 AI Agent:**
> The average net burn is 8.5, and the burn trend is increasing with a volatility index of 1.2.


## ❓ FAQ

**Q: How does this tool calculate the projected runway?**
The `project_runway` tool uses current cash reserves and historical net burn values to estimate the number of months remaining before cash is exhausted.

**Q: Can I detect unusual spending spikes?**
Yes, the `identify_anomalies` tool detects one-time expenses or revenue spikes that deviate from the historical average.

**Q: What is the difference between gross and net burn?**
Gross burn is the total monthly outflow, while net burn is the actual monthly deficit after subtracting revenue. You can find these values using `get_current_burn_metrics`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/burn-rate-analysis](https://vinkius.com/en/ai-agent-connect/burn-rate-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Burn Rate Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `burn-rate-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Burn Rate Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "burn-rate-analysis": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
