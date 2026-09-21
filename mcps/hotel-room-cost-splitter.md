# Hotel Room Cost Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hotel-room-cost-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Equitable cost distribution for shared accommodations.

## Description
This MCP server provides precise financial tools to split hotel and vacation rental costs among travelers. It accounts for complex variables including nights occupied, room types, taxes, cleaning fees, and discounts. Use `get_cost_distribution` to calculate proportional shares based on stay duration and custom fairness weights, `get_payment_schedule` to generate debt settlement transfers, and `get_reconciliation_report` to handle rounding residuals. It ensures every cent is accounted for in shared stays.


## Available Tools (4)
- **get_payment_schedule**: Generates a list of transfers needed to settle the debt between travelers
- **get_reconciliation_report**: Provides a final summary of the total cost, individual responsibilities, and the final adjustment needed for rounding
- **get_stay_summary**: Provides a high-level overview of the stay metrics (cost per night, tax impact, etc.)
- **get_cost_distribution**: Calculates the primary breakdown of how much each person owes based on stay duration and fairness weights


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hotel Room Cost Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Split a $500 room cost with a $50 cleaning fee and 10% tax between Alice (3 nights) and Bob (2 nights)."

**🤖 AI Agent:**
> Alice's share is $330.00 and Bob's share is $220.00.

---

**👤 You:**
> "Generate a payment schedule for Alice who owes $100 and Bob who already paid $100."

**🤖 AI Agent:**
> Alice should transfer $100.00 to Bob.

---

**👤 You:**
> "What is the cost per night for a $1000 room with a 10% tax and $100 cleaning fee for 4 nights?"

**🤖 AI Agent:**
> The cost per night is $300.00.


## ❓ FAQ

**Q: How does the tool handle different stay lengths?**
The `get_cost_distribution` tool uses the number of nights stayed by each person to calculate their proportional share of the total cost.

**Q: Can I make certain people pay more or less?**
Yes, you can use fairness weights in `get_cost_distribution` to adjust a person's share regardless of their stay duration.

**Q: How are rounding errors handled?**
You can use `get_reconciliation_report` to identify the residual difference caused by currency rounding and assign it to a designated leader.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hotel-room-cost-splitter](https://vinkius.com/en/ai-agent-connect/hotel-room-cost-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hotel Room Cost Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hotel-room-cost-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hotel Room Cost Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hotel-room-cost-splitter": {
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
