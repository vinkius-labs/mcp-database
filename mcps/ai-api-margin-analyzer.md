# AI API Margin Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ai-api-margin-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze profitability and optimal pricing structures for AI API usage tiers.

## Description
This MCP server provides specialized tools for evaluating the profitability of AI API pricing models. It allows users to calculate margins across different usage tiers, evaluate the impact of commit discounts and overage pricing, and suggest optimal tier structures to maximize profit. Use `analyze_tier_margins` to find the profitability of specific tiers, or `recommend_optimal_structure` to find the best configuration for a target margin.


## Available Tools (4)
- **analyze_tier_margins**: Calculates the individual profitability percentage for each defined pricing tier
- **calculate_discount_impact**: Evaluates how much revenue and margin are sacrificed when applying commit discounts and overage pricing
- **get_usage_summary**: Provides a high-level overview of how usage volume is distributed across the tiers
- **recommend_optimal_structure**: Suggests the best pricing tier thresholds and unit prices to maximize total profit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AI API Margin Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the margin for my current tiers?"

**🤖 AI Agent:**
> The margin for the Standard Tier is 45%, the Growth Tier is 38%, and the Enterprise Tier is 52%.

---

**👤 You:**
> "Show me a summary of my usage distribution."

**🤖 AI Agent:**
> Total volume is 1,500 units. The primary tier is the Growth Tier, which accounts for 60% of the total volume.

---

**👤 You:**
> "How much revenue do I lose by offering a 10% commit discount?"

**🤖 AI Agent:**
> The total discount loss is $5,000, resulting in an effective margin reduction of 4.2%.


## ❓ FAQ

**Q: How do I calculate margins for my current pricing model?**
You can use the `analyze_tier_margins` tool. Provide your pricing tiers, usage distribution, compute costs, and total support cost to receive a detailed breakdown of revenue and profit per tier.

**Q: Can this tool help me find the best pricing tiers?**
Yes, the `recommend_optimal_structure` tool simulates different tier configurations to find the one that maximizes total profit while meeting your target margin.

**Q: How does the tool account for volume discounts?**
The `calculate_discount_impact` tool specifically evaluates how much revenue and margin are sacrificed when applying commit discounts and overage pricing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ai-api-margin-analyzer](https://vinkius.com/ai-agent-connect/ai-api-margin-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AI API Margin Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ai-api-margin-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AI API Margin Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ai-api-margin-analyzer": {
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
