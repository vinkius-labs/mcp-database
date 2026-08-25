# Accelerator Management Fee Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-management-fee-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate management fee structures, investable capital, and fee drag for accelerator funds.

## Description
This MCP server provides specialized tools for venture capital and accelerator fund managers to model fee structures. Use `calculate_fee_structure` to determine annual fee amounts and total costs over a fund's life, including step-down schedules. Use `calculate_investable_capital` to find the net capital available for deployment after fees and recycling. Finally, use `calculate_fee_drag` to quantify the percentage impact of management fees on deployment capability.


## Available Tools (3)
- **calculate_fee_drag**: calculate_fee_drag
- **calculate_fee_structure**: Determines annual fee amounts and total fees
- **calculate_investable_capital**: calculate_investable_capital


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Management Fee Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total fees for a $50M fund with a 2% annual fee over 10 years."

**🤖 AI Agent:**
> The total management fees for a $50,000,000 fund over 10 years at a 2% annual rate is $10,000,000.

---

**👤 You:**
> "How much investable capital is left in a $20M fund if total fees are $2M and we recycle $1M?"

**🤖 AI Agent:**
> The investable capital available for deployment is $19,000,000.

---

**👤 You:**
> "What is the fee drag for a $100M fund with $5M in total fees?"

**🤖 AI Agent:**
> The fee drag is 5.0%.


## ❓ FAQ

**Q: How does the fee basis affect calculations?**
The fee basis determines if fees are applied to the total committed capital or the actual capital deployed. You can specify this using the `feeBasis` parameter in `calculate_fee_structure`.

**Q: Can I model declining fees over time?**
Yes, you can provide a step-down schedule to `calculate_fee_structure` to define specific fee rates for each year of the fund's life.

**Q: What is fee drag?**
Fee drag is the percentage of the fund's total size that is consumed by management fees instead of being invested in companies. You can calculate this with `calculate_fee_drag`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-management-fee-calculator](https://vinkius.com/ai-agent-connect/accelerator-management-fee-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Management Fee Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-management-fee-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Management Fee Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-management-fee-calculator": {
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
