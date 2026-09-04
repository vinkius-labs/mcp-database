# Enterprise Renewal Expansion Rate MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-renewal-expansion-rate)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates revenue expansion metrics and upsell opportunities during enterprise contract renewals.

## Description
This MCP server provides a financial calculation engine to determine the percentage and dollar value of revenue expansion during enterprise contract renewals. It uses `calculate_expansion_metrics` to find growth rates, `evaluate_expansion_type` to distinguish between upsell and cross-sell, and `project_upsell_opportunity` to estimate remaining revenue potential. It is designed to help sales and finance teams track expansion health and negotiation progress.


## Available Tools (4)
- **calculate_expansion_metrics**: Calculates the core expansion percentage and dollar amount for a specific renewal
- **evaluate_expansion_type**: Categorizes the nature of the growth to assist in sales reporting
- **get_renewal_summary**: Provides a consolidated view of a single renewal's health and expansion performance
- **project_upsell_opportunity**: Estimates the remaining revenue potential during the negotiation phase


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Renewal Expansion Rate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the expansion metrics for a renewal with a base ARR of 100000 and an expanded ARR of 125000."

**🤖 AI Agent:**
> The expansion rate is 25% and the expansion at renewal is $25,000.

---

**👤 You:**
> "What is the upsell opportunity for a contract with 50000 base ARR, 60000 expanded ARR, and currently in early_negotiation stage?"

**🤖 AI Agent:**
> The projected upsell value is $15,000 with low confidence due to the early negotiation stage.

---

**👤 You:**
> "Get a summary for a renewal: base ARR 200000, expanded ARR 250000, type is upsell, and stage is finalizing."

**🤖 AI Agent:**
> The renewal summary shows a 25% expansion rate, $50,000 expansion amount, categorized as upsell, in the finalizing stage.


## ❓ FAQ

**Q: What is the difference between upsell and cross-sell in this tool?**
Using `evaluate_expansion_type`, the tool identifies 'upsell' as volume-based growth of existing products and 'cross-sell' as the addition of entirely new product lines.

**Q: How can I estimate potential revenue before a contract is signed?**
You can use `project_upsell_opportunity` to estimate the remaining revenue potential based on the current negotiation stage.

**Q: Does this tool support different renewal stages?**
Yes, the tools account for different phases such as early negotiation, finalizing, and closed stages to provide accurate metrics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-renewal-expansion-rate](https://vinkius.com/ai-agent-connect/enterprise-renewal-expansion-rate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Renewal Expansion Rate** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-renewal-expansion-rate` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Renewal Expansion Rate** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-renewal-expansion-rate": {
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
