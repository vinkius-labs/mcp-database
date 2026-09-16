# Venture Deal Sourcing Efficiency MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-deal-sourcing-efficiency)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze and optimize venture capital deal sourcing ROI and channel performance.

## Description
This MCP server provides specialized analytical tools for venture capital firms to measure the financial and temporal efficiency of their deal-sourcing channels. By integrating monetary costs with human capital time-investment, it calculates precise metrics like Cost Per Deal and Conversion Rate. Use `get_channel_roi` to incorporate qualitative factors like deal quality and relationship value into your ROI calculations, or `get_aggregate_sourcing_efficiency` for a high-level overview of your entire sourcing engine. It is designed to help firms identify their most effective sourcing methods through `compare_channel_efficiency`.


## Available Tools (4)
- **get_aggregate_sourcing_efficiency**: Provides a high-level overview of the entire sourcing operation across all channels
- **get_channel_performance**: Calculates the core efficiency metrics (Cost Per Deal and Conversion Rate) for a specific sourcing channel
- **get_channel_roi**: Determines the Return on Investment for a specific channel, incorporating qualitative value
- **compare_channel_efficiency**: Ranks and compares different channels to identify the most and least effective sourcing methods


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Deal Sourcing Efficiency** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the cost per deal for the 'Direct Outbound' channel if we spent $5000 and 100 hours at $150/hr to find 5 deals?"

**🤖 AI Agent:**
> The cost per deal for the Direct Outbound channel is $3,500.

---

**👤 You:**
> "Compare the efficiency of 'Networking' and 'Events' based on their performance data."

**🤖 AI Agent:**
> Networking is your top performing channel with an ROI of 2.5, while Events is the least efficient with a Cost Per Deal of $8,000.

---

**👤 You:**
> "Give me a summary of our total sourcing efficiency across all channels."

**🤖 AI Agent:**
> Your total sourcing cost is $45,000 for 12 deals, resulting in an average cost per deal of $3,750 and a global efficiency score of 0.85.


## ❓ FAQ

**Q: How does the tool account for human labor costs?**
The system uses Time-Cost Equivalence. By providing an `hourlyRate`, the tool converts hours spent on sourcing into a monetary value, which is then added to direct monetary costs to calculate the true total channel cost.

**Q: Can I compare different sourcing channels?**
Yes, you can use `compare_channel_efficiency` to rank channels based on their ROI and Cost Per Deal, helping you identify your top-performing and least efficient methods.

**Q: How is ROI calculated for a specific channel?**
The `get_channel_roi` tool calculates ROI by adjusting performance metrics with a deal quality multiplier and a relationship value score, providing a multi-dimensional view of channel effectiveness.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-deal-sourcing-efficiency](https://vinkius.com/en/ai-agent-connect/venture-deal-sourcing-efficiency)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Deal Sourcing Efficiency** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-deal-sourcing-efficiency` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Deal Sourcing Efficiency** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-deal-sourcing-efficiency": {
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
