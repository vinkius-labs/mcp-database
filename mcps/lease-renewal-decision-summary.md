# Lease Renewal Decision Summary MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/lease-renewal-decision-summary)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare the costs of staying in your current lease versus moving to a new residence.

## Description
This MCP server provides a financial comparison engine to evaluate the economic impact of renewing an existing lease versus moving. It calculates cumulative costs including rent, moving fees, security deposits, and the financial impact of commute changes. Use `calculate_stay_costs` to find the cost of staying, `calculate_move_costs` for relocation expenses, and `compare_options` to identify the break-even month where moving becomes more cost-effective.


## Available Tools (4)
- **calculate_commute_delta**: Calculate commute delta
- **calculate_move_costs**: Calculate move costs
- **calculate_stay_costs**: Calculate stay costs
- **compare_options**: Compare stay vs move


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lease Renewal Decision Summary** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'm staying in my current place for $2000/month for 12 months. If I move, the new rent is $1800, moving fees are $500, and the deposit is $1800. My commute will increase by 15 minutes daily, and my time is worth $30/hour. I work 20 days a month. Compare the options."

**🤖 AI Agent:**
> The total cost to stay is $24,000. The total cost to move is $25,700. There is no break-even month within the 12-month horizon as staying remains the cheaper option.

---

**👤 You:**
> "Calculate the cost of staying with a $2500 rent for 24 months."

**🤖 AI Agent:**
> The total cumulative cost for staying is $60,000.

---

**👤 You:**
> "What is the financial impact of a 20-minute increase in my daily commute if I work 22 days a month, my time is worth $25 per hour, and I'm looking at a 12-month horizon?"

**🤖 AI Agent:**
> The total commute cost for the 12-month period is $1,100.


## ❓ FAQ

**Q: How does the tool calculate the break-even month?**
The break-even month is identified by `compare_options` as the first month where the cumulative cost of moving becomes lower than the cumulative cost of staying within your specified time horizon.

**Q: Can I include commute changes in my comparison?**
Yes, you can use `calculate_commute_delta` to quantify the financial impact of changes in commute time, which is then factored into the final comparison.

**Q: What costs are included in the moving calculation?**
The `calculate_move_costs` tool includes the new monthly rent, one-time moving fees (movers, packing, utilities), and the new security deposit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/lease-renewal-decision-summary](https://vinkius.com/en/ai-agent-connect/lease-renewal-decision-summary)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lease Renewal Decision Summary** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lease-renewal-decision-summary` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lease Renewal Decision Summary** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lease-renewal-decision-summary": {
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
