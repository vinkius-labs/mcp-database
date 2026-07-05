# Moving Cost Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moving-cost-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare the financial impact of DIY truck rentals versus professional full-service moving companies.

## Description
The Moving Cost Comparator is a decision-support engine designed to help you evaluate the economic trade-offs between self-managed moves and professional services. Using tools like `calculate_diy_costs`, `calculate_full_service_costs`, and `analyze_moving_comparison`, you can project total expenditures for truck rentals, fuel, and equipment against the baseline fees of professional movers. The engine identifies your 'break-even' point--the exact number of labor hours where hiring a crew becomes more expensive than doing it yourself.


## Available Tools (3)
- **analyze_moving_comparison**: Provides the definitive comparison between the two moving strategies
- **calculate_diy_costs**: Calculates the total projected expenditure for a self-managed move
- **calculate_full_service_costs**: Calculates the total projected cost for hiring professional movers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moving Cost Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will a DIY move cost if I rent a MEDIUM truck for 300 miles, with 15 MPG and gas at $3.50/gallon, plus $50 for gear?"

**🤖 AI Agent:**
> $260.00

---

**👤 You:**
> "Calculate the full-service cost for an ESTATE move with a 100 mile travel distance, $500 travel fee, and $200 insurance premium."

**🤖 AI Agent:**
> $1200.00

---

**👤 You:**
> "If my DIY total is $500 and the professional baseline (travel + insurance) is $300 with an hourly rate of $40, what is my break-even point?"

**🤖 AI Agent:**
> 5.0 hours


## ❓ FAQ

**Q: How does the DIY cost calculation work?**
The `calculate_diy_costs` tool aggregates your truck rental base rate (based on size and distance), fuel consumption costs, equipment rentals like dollies or pads, and any planned refreshment costs for helpers.

**Q: What is the 'break-even' point?**
The break-even point, calculated via `analyze_moving_comparison`, represents the maximum number of labor hours you can afford to hire a professional crew before their service cost exceeds your DIY budget.

**Q: Does this tool include fuel prices?**
Yes, when using `calculate_diy_costs`, you provide the current price per unit of fuel and the truck's estimated efficiency to get an accurate projection.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moving-cost-comparator](https://vinkius.com/mcp/moving-cost-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moving Cost Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moving-cost-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moving Cost Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moving-cost-comparator": {
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
