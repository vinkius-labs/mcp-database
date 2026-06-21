# Tax Loss Harvesting Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tax-loss-harvesting-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate the financial benefits and tax savings from harvesting capital losses.

## Description
This MCP server provides specialized tools to calculate the economic impact of tax-loss harvesting. Use `evaluate_harvesting_opportunity` to determine avoided taxes and net savings after reinvestment friction. You can also use `get_wash_sale_window` to check compliance periods for different jurisdictions like the USA or Germany, and `retrieve_tax_rate_by_jurisdiction` to find applicable capital gains rates based on your location and income band.


## Available Tools
- **evaluate_harvesting_opportunity**: Calculates the potential tax benefits and net economic impact of harvesting losses
- **retrieve_tax_rate_by_jurisdiction**: Retrieves the correct capital gains percentage based on jurisdiction and income band
- **get_wash_sale_window**: Determines the regulatory window for wash sale compliance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tax Loss Harvesting Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my tax savings if I have a loss of $5000 with a 15% tax rate and $50 in fees."

**🤖 AI Agent:**
> The total avoided tax is $750.00, and your net savings after the $50.00 friction cost is $700.00.

---

**👤 You:**
> "What is the wash sale window in Germany?"

**🤖 AI Agent:**
> The wash sale window for Germany is 0 days.

---

**👤 You:**
> "What capital gains rate applies to me in the USA if I am in the medium income band?"

**🤖 AI Agent:**
> The applicable capital gains tax rate for the medium income band in the USA is 15%.


## ❓ FAQ

**Q: How do I calculate my potential tax savings?**
Use the `evaluate_harvesting_opportunity` tool by providing your current positions, the applicable tax rate, and any reinvestment friction costs.

**Q: What is the wash sale rule window for the USA?**
For the USA, the `get_wash_sale_window` tool confirms a 30-day period surrounding the transaction where you must avoid repurchasing substantially identical securities.

**Q: Can I retrieve tax rates for European countries?**
Yes, use `retrieve_tax_rate_by_jurisdiction` to get the flat capital gains rate for supported EU nations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tax-loss-harvesting-calculator](https://vinkius.com/mcp/tax-loss-harvesting-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tax Loss Harvesting Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `tax-loss-harvesting-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tax Loss Harvesting Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tax-loss-harvesting-calculator": {
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
