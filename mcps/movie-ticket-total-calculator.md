# Movie Ticket Total Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/movie-ticket-total-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate movie admission costs with tiered pricing and group discounts.

## Description
This MCP server provides specialized tools for calculating movie ticket costs. Use `calculate_basic_total` for simple attendee counts, `calculate_tiered_total` to manage different age demographics like adults, children, and seniors, and `apply_group_discount` to reduce the final price for large groups. You can also use `get_pricing_tier_info` to retrieve standard regional pricing for areas like the USA or Europe.


## Available Tools (4)
- **apply_group_discount**: 
- **calculate_tiered_total**: 
- **calculate_basic_total**: 
- **get_pricing_tier_info**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Movie Ticket Total Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will it cost for 5 people if the base price is $12?"

**🤖 AI Agent:**
> The total cost for 5 people at a base price of $12 is $60.

---

**👤 You:**
> "Calculate the total for 2 adults at $15, 1 child at $10, and 1 senior at $8."

**🤖 AI Agent:**
> The total cost is $48, with a breakdown of $30 for adults, $10 for children, and $8 for seniors.

---

**👤 You:**
> "If the total is $100 and I have a group of 10 people, can I get a 10% discount if the threshold is 5 people?"

**🤖 AI Agent:**
> Yes, the final total after the 10% discount is $90.


## ❓ FAQ

**Q: How do I calculate costs for different age groups?**
You can use the `calculate_tiered_total` tool, which accepts counts and prices for adults, children, and seniors to provide a full breakdown.

**Q: Can I apply discounts for large groups?**
Yes, use the `apply_group_discount` tool to apply a percentage reduction if the group size meets your specified threshold.

**Q: Where can I find standard regional prices?**
Use the `get_pricing_tier_info` tool and specify a region like 'USA' or 'Europe' to retrieve the current standard pricing tiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/movie-ticket-total-calculator](https://vinkius.com/en/ai-agent-connect/movie-ticket-total-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Movie Ticket Total Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `movie-ticket-total-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Movie Ticket Total Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "movie-ticket-total-calculator": {
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
