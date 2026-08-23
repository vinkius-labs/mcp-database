# Insulin on Board Decay Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/insulin-on-board-decay-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate remaining active insulin and assess stacking risk.

## Description
This MCP server provides deterministic tools to calculate Insulin on Board (IOB) using a linear decay model. It helps prevent insulin stacking by assessing the risk of hypoglycemia. Use `calculate_iob_metrics` to find current insulin levels and predicted blood glucose lowering potential, or `assess_stacking_risk` to check if a new dose is safe. You can also use `get_iob_at_specific_times` to project future insulin levels.


## Available Tools (3)
- **assess_stacking_risk**: Assess the risk of insulin stacking
- **calculate_iob_metrics**: Calculate current insulin on board and its decay profile
- **get_iob_at_specific_times**: Project insulin levels at specific future time points


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Insulin on Board Decay Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I took 5 units of insulin 60 minutes ago. The duration is 240 minutes and my ISF is 50. What is my current IOB and risk?"

**🤖 AI Agent:**
> Your current IOB is 3.75 units. The effective blood glucose lowering potential is 187.5 mg/dL. Your stacking risk is High Stacking Risk.

---

**👤 You:**
> "Check if I can take more insulin. I have 0.2 units of insulin left from a dose taken 200 minutes ago."

**🤖 AI Agent:**
> Your stacking risk is Low Stacking Risk.

---

**👤 You:**
> "What will my insulin levels be in 30 and 60 minutes if I took 4 units 30 minutes ago with a 240 minute duration?"

**🤖 AI Agent:**
> In 30 minutes (60 mins total), your IOB will be 3.0 units. In 60 minutes (90 mins total), your IOB will be 2.25 units.


## ❓ FAQ

**Q: How is the insulin decay calculated?**
The server uses a linear decay model where insulin activity decreases at a constant rate until it reaches zero at the end of its duration of action.

**Q: What is insulin stacking?**
Insulin stacking occurs when a new dose is administered before the previous dose has finished its activity, which can lead to severe hypoglycemia.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/insulin-on-board-decay-calculator](https://vinkius.com/ai-agent-connect/insulin-on-board-decay-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Insulin on Board Decay Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `insulin-on-board-decay-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Insulin on Board Decay Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "insulin-on-board-decay-calculator": {
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
