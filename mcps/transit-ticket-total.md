# Transit Ticket Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/transit-ticket-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates transit fare costs based on passenger types and group volume.

## Description
This MCP server provides a specialized calculation engine for transit authorities and travel planners. It determines total fare costs by processing passenger counts, applying specific classification discounts for adults, children, and seniors, and calculating volume-based group discounts. Use `get_single_ticket_price` to check individual rates, `calculate_group_total` for group sums, `apply_group_discount` to find volume savings, or `get_fare_breakdown` for a full audit of the final price.


## Available Tools (4)
- **apply_group_discount**: Answers how much of a discount should be applied based on the total number of people traveling
- **calculate_group_total**: Answers what the total cost is for a specific group of passengers
- **get_fare_breakdown**: Answers for a detailed audit of how the final total was reached
- **get_single_ticket_price**: Answers how much a single passenger of a specific type will pay


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Transit Ticket Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will 2 adults and 1 child pay if the base fare is 10.00?"

**🤖 AI Agent:**
> The total cost for 2 adults and 1 child with a base fare of 10.00 is 25.00.

---

**👤 You:**
> "What is the price for a single senior passenger with a base fare of 15.00?"

**🤖 AI Agent:**
> A single senior passenger will pay 10.50.

---

**👤 You:**
> "How much discount is applied for a group of 10 people?"

**🤖 AI Agent:**
> A group of 10 people qualifies for a significant volume discount.


## ❓ FAQ

**Q: How do I calculate the total for a group?**
You can use the `calculate_group_total` tool by providing the passenger counts for each type and the base fare.

**Q: Can I see a detailed breakdown of the costs?**
Yes, the `get_fare_breakdown` tool provides a detailed audit including individual category totals and applied group discounts.

**Q: What passenger types are supported?**
The system supports adult, child, and senior classifications for fare calculation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/transit-ticket-total](https://vinkius.com/en/ai-agent-connect/transit-ticket-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Transit Ticket Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `transit-ticket-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Transit Ticket Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "transit-ticket-total": {
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
