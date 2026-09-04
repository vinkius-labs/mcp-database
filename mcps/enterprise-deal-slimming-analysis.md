# Enterprise Deal Slimming Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-deal-slimming-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [revenue-operations](../categories/revenue-operations.md)

Analyze deal size reduction patterns and procurement impact.

## Description
This MCP server provides tools to identify where and why sales value is lost during the enterprise procurement process. Use `analyze_overall_slimming` to calculate total value loss, `get_stage_specific_reduction` to find which sales stage causes the most reduction, `identify_negotiation_drivers` to compare procurement tactics against competitive pressure, and `detect_discount_anomalies` to find unusual discounting patterns.


## Available Tools (4)
- **get_stage_specific_reduction**: Identifies which sales stage experiences the most value reduction
- **analyze_overall_slimming**: Calculates the total percentage of value lost across a set of deals
- **detect_discount_anomalies**: Detects unusual discount patterns relative to deal size
- **identify_negotiation_drivers**: Determines the impact of procurement tactics vs competitive pressure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Deal Slimming Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the total percentage of value lost across these deals: [{'initialSize': 100000, 'closedSize': 80000}, {'initialSize': 50000, 'closedSize': 45000}]?"

**🤖 AI Agent:**
> The average slimming percentage is 15% and the total value lost is $25,000.

---

**👤 You:**
> "Which stage had the highest reduction: [{'stage': 'Discovery', 'initialSize': 100000, 'closedSize': 95000}, {'stage': 'Negotiation', 'initialSize': 100000, 'closedSize': 70000}]?"

**🤖 AI Agent:**
> The highest reduction stage is Negotiation.

---

**👤 You:**
> "Compare the impact of procurement vs competition for this deal: [{'initialSize': 100000, 'closedSize': 80000, 'procurementLoss': 15000, 'competitionLoss': 5000}]"

**🤖 AI Agent:**
> Procurement impact is 75% and competition impact is 25%, with a total attributed loss of $20,000.


## ❓ FAQ

**Q: What is deal slimming?**
Deal slimming is the reduction in contract value from the initial proposed amount to the final signed amount, often driven by procurement tactics or competition.

**Q: How can I identify which sales stage is most problematic?**
You can use the `get_stage_specific_reduction` tool to analyze value loss across different stages of your sales cycle.

**Q: Can this tool detect unusual discounts?**
Yes, the `detect_discount_anomalies` tool identifies deals where the discount applied deviates significantly from the average.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-deal-slimming-analysis](https://vinkius.com/ai-agent-connect/enterprise-deal-slimming-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Deal Slimming Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-deal-slimming-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Deal Slimming Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-deal-slimming-analysis": {
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
