# Life Events Stress Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/life-events-stress-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Assess cumulative psychological stress risks using the Holmes-Rahe Scale.

## Description
This MCP server implements the Holmes-Rahe Stress Adaptation model. By quantifying recent life events into Life Change Units (LCU), it calculates your total accumulated stress load and identifies potential health risks. Use `get_available_events` to see supported changes, `calculate_stress_score` to compute your risk level based on specific event IDs, and `get_risk_thresholds` to understand the scoring tiers.


## Available Tools (3)
- **get_available_events**: Can filter by category (Critical, Moderate, Minor).

See which life events are supported and their weights
- **calculate_stress_score**: Compute total stress score and risk level
- **get_risk_thresholds**: Get definitions of risk categories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Life Events Stress Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What life events can I track for stress calculation?"

**🤖 AI Agent:**
> You can track various events including bereavement, divorce, job changes, and more. Use `get_available_events` to see the full list and their weights.

---

**👤 You:**
> "Calculate my stress score if I've experienced a death in the family and a job change."

**🤖 AI Agent:**
> Based on those events, your total LCU score is 210, which places you in the High Risk category.

---

**👤 You:**
> "What are the risk thresholds for this tool?"

**🤖 AI Agent:**
> The risk tiers are: Low Risk (0-149), Moderate Risk (150-299), and High Risk (300+).


## ❓ FAQ

**Q: How is the stress score calculated?**
The tool assigns a specific weight (Life Change Units) to each life event. The total score is the sum of all weights from the events you provide via `calculate_stress_score`.

**Q: What does a high risk level mean?**
A high risk level indicates that the cumulative stress from recent life changes is substantial enough to significantly increase the likelihood of physical or mental health strain.

**Q: Can I filter events by category?**
Yes, you can use the `categoryFilter` parameter in the `get_available_events` tool to view only Critical, Moderate, or Minor events.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/life-events-stress-calculator](https://vinkius.com/mcp/life-events-stress-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Life Events Stress Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `life-events-stress-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Life Events Stress Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "life-events-stress-calculator": {
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
