# Enterprise Upsell Cycle Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-upsell-cycle-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [revenue-operations](../categories/revenue-operations.md)

Predict upsell timelines, velocity, and acceleration strategies for enterprise accounts.

## Description
This MCP server provides advanced modeling for enterprise expansion opportunities. It calculates predicted upsell cycles by weighing opportunity size against customer tenure and trust levels. Use `calculate_cycle_metrics` to get a full overview of timeline and momentum, `get_velocity_benchmarks` to compare deal speed against performance tiers, and `recommend_acceleration_tactics` to identify specific actions to shorten sales cycles. It also includes `evaluate_relationship_impact` to quantify how existing customer relationships affect friction in the sales process.


## Available Tools (4)
- **calculate_cycle_metrics**: Provides a comprehensive overview of the predicted timeline and momentum for a specific upsell opportunity
- **evaluate_relationship_impact**: Determines how much the existing customer relationship is currently helping or hindering the sales process
- **get_velocity_benchmarks**: Compares a specific deal's velocity against standard performance tiers for the same upsell type
- **recommend_acceleration_tactics**: Generates specific business actions to shorten the cycle when the predicted duration exceeds a target threshold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Upsell Cycle Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the metrics for a $50,000 seat expansion with a 24-month tenure and a trust level of 4 under standard approval."

**🤖 AI Agent:**
> The predicted average cycle is 45 days with a high velocity score of 0.85.

---

**👤 You:**
> "The predicted upsell cycle is 90 days, but my target is 60 days for this feature upgrade. What should I do?"

**🤖 AI Agent:**
> To reduce the cycle time, you should prioritize 'Value Realization Proof' to address the size-based delay.

---

**👤 You:**
> "How much is our 36-month relationship and trust level of 5 helping us right now?"

**🤖 AI Agent:**
> The relationship impact analysis shows a low friction coefficient of 0.2, indicating a very strong relationship that significantly accelerates the process.


## ❓ FAQ

**Q: How does this tool help my sales team?**
It provides data-driven predictions on how long an upsell deal will take and offers specific tactics to speed up the process using `recommend_acceleration_tactics`.

**Q: Can I compare my current deal velocity to industry standards?**
Yes, by using `get_velocity_benchmarks`, you can see if your current deal's momentum is high, stable, or stagnant compared to typical performance for that upsell type.

**Q: What factors influence the predicted upsell cycle?**
The cycle is influenced by the opportunity size, the complexity of the approval process, customer tenure, and the current trust level with the client.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-upsell-cycle-analyzer](https://vinkius.com/ai-agent-connect/enterprise-upsell-cycle-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Upsell Cycle Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-upsell-cycle-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Upsell Cycle Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-upsell-cycle-analyzer": {
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
