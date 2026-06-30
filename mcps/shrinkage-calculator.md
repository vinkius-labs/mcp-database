# Shrinkage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shrinkage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate inventory shrinkage, risk levels, and security investment ROI.

## Description
The Shrinkage Calculator MCP server provides specialized tools for analyzing inventory loss. Use `calculate_shrinkage_metrics` to determine absolute and percentage shrinkage, identify risk tiers (Acceptable, Warning, or Critical), and project annual losses. The `analyze_security_breakeven` tool helps evaluate the financial viability of security measures by calculating projected savings and payback periods. Additionally, `get_risk_thresholds` allows you to retrieve the current business rules for shrinkage classification.


## Available Tools (3)
- **get_risk_thresholds**: Retrieve shrinkage risk thresholds
- **analyze_security_breakeven**: Analyze financial viability of security investment
- **calculate_shrinkage_metrics**: Calculate inventory shrinkage metrics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shrinkage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate shrinkage metrics for a period where initial stock was $10,000, purchases were $5,000, final stock is $14,000, and recorded COGS was $6,000."

**🤖 AI Agent:**
> Absolute shrinkage: $1,000. Shrinkage percentage: 4.76%. Risk classification: Critical. Annualized loss: $12,000.

---

**👤 You:**
> "If my annual shrinkage loss is $50,000 and a new security system costs $10,000 per year with an expected 30% reduction, what is the payback period?"

**🤖 AI Agent:**
> Projected annual savings: $15,000. Net annual benefit: $5,000. Payback period: 24 months.

---

**👤 You:**
> "What are the current risk thresholds for shrinkage?"

**🤖 AI Agent:**
> The thresholds are: Low (Acceptable) up to 1.5%, Medium (Warning) up to 3%, and High (Critical) above 3%.


## ❓ FAQ

**Q: What is inventory shrinkage?**
Shrinkage refers to the loss of inventory due to theft, damage, administrative errors, or fraud. It is the difference between recorded stock and actual physical stock.

**Q: How can I calculate the ROI of a security camera installation?**
You can use the `analyze_security_breakeven` tool. Provide your annualized shrinkage loss, the annual cost of the cameras, and the expected reduction rate to see the projected savings and payback period.

**Q: What are the risk thresholds used for classification?**
The tool uses hardcoded business rules. You can retrieve these specific boundaries using the `get_risk_thresholds` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shrinkage-calculator](https://vinkius.com/mcp/shrinkage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shrinkage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shrinkage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shrinkage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shrinkage-calculator": {
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
