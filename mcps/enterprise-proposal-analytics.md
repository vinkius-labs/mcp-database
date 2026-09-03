# Enterprise Proposal Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-proposal-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [enterprise](../categories/enterprise.md)

Calculate key performance indicators for enterprise sales proposals.

## Description
This MCP server provides analytical tools to measure enterprise sales effectiveness. It allows AI agents to calculate win rates using `calculate_win_rate_metrics`, assess financial impact with `calculate_proposal_value_metrics`, measure sales velocity via `calculate_cycle_time_metrics`, and evaluate market risk through `analyze_competitive_positioning`.


## Available Tools (4)
- **analyze_competitive_positioning**: Evaluate how pricing and competition influence success likelihood
- **calculate_cycle_time_metrics**: Measure the speed of the sales process
- **calculate_proposal_value_metrics**: Assess the financial impact of proposal activities
- **calculate_win_rate_metrics**: Calculate fundamental efficiency of the proposal pipeline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Proposal Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my current win rate if I sent 50 proposals and won 15?"

**🤖 AI Agent:**
> Your current win rate is 30%.

---

**👤 You:**
> "Calculate the average value of my won proposals: [10000, 25000, 15000]."

**🤖 AI Agent:**
> The average value of your won proposals is $16,666.67.

---

**👤 You:**
> "How long does it take to close deals? The durations are 10, 20, and 30 days."

**🤖 AI Agent:**
> The average cycle time is 20 days, with the fastest close at 10 days and the slowest at 30 days.


## ❓ FAQ

**Q: How do I calculate my sales win rate?**
You can use the `calculate_win_rate_metrics` tool by providing the total number of proposals sent and the number of proposals won.

**Q: Can I assess market risk based on my pricing strategy?**
Yes, the `analyze_competitive_positioning` tool evaluates risk levels by considering your pricing strategy, competitor density, and positioning strength.

**Q: How is sales velocity measured?**
Sales velocity is measured using `calculate_cycle_time_metrics`, which analyzes the duration from proposal submission to final decision.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-proposal-analytics](https://vinkius.com/ai-agent-connect/enterprise-proposal-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Proposal Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-proposal-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Proposal Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-proposal-analytics": {
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
