# Affiliate Commission Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/affiliate-commission-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate accurate affiliate payouts with regional tax adjustments.

## Description
This MCP server provides a specialized calculation engine for determining affiliate commissions. It handles single sale calculations using `calculate_single_commission`, manages volume-based payouts via `get_tiered_commission`, ensures regulatory alignment with `validate_regional_compliance`, and processes bulk transactions through `batch_calculate_commissions`. The engine automatically accounts for regional tax multipliers in the USA and EU to ensure accurate net payouts.


## Available Tools (4)
- **batch_calculate_commissions**: Calculate total payout for multiple sales
- **calculate_single_commission**: Calculate commission for a single sale
- **get_tiered_commission**: Calculate commission based on volume thresholds
- **validate_regional_compliance**: Validate if a commission is compliant with regional rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Affiliate Commission Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the commission for a sale of $500 with a 10% rate in the USA."

**🤖 AI Agent:**
> The commission amount is $50.00 and the net commission after USA regional adjustments is $45.00.

---

**👤 You:**
> "What is the commission for a $1200 sale using these tiers: [{'threshold': 1000, 'rate': 15}, {'threshold': 500, 'rate': 10}] in the EU?"

**🤖 AI Agent:**
> The applied rate is 15%, resulting in a commission amount of $180.00 and a net commission of $162.00 after EU adjustments.

---

**👤 You:**
> "Check if a $100 commission is compliant in the EU."

**🤖 AI Agent:**
> The commission is compliant with regional rules, with an adjustment factor applied for VAT considerations.


## ❓ FAQ

**Q: How does the engine handle regional taxes?**
The engine uses regional multipliers to adjust the gross commission into a net commission, accounting for specific tax rules in the USA and EU.

**Q: Can I calculate commissions for multiple sales at once?**
Yes, you can use the `batch_calculate_commissions` tool to process an array of sales and get an aggregated total payout.

**Q: What happens if a sale amount is below the lowest tier?**
When using `get_tiered_commission`, if the sale amount does not meet any defined threshold, a base rate of zero is applied.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/affiliate-commission-engine](https://vinkius.com/en/ai-agent-connect/affiliate-commission-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Affiliate Commission Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `affiliate-commission-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Affiliate Commission Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "affiliate-commission-engine": {
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
