# match-ticket-total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/match-ticket-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculates total ticket costs based on attendee counts and pricing tiers.

## Description
This MCP server provides tools to manage ticket pricing and booking eligibility. Use `calculate_total_cost` to find the aggregate price for a group, `get_tier_price` to determine the unit cost for a specific number of attendees, `validate_booking_eligibility` to check if a group size is allowed, and `list_pricing_structure` to view all available pricing tiers.


## Available Tools (4)
- **calculate_total_cost**: Calculates the final aggregate cost for a group of attendees
- **get_tier_price**: Determines the applicable price per ticket for a given number of attendees
- **list_pricing_structure**: Provides an overview of the current available pricing tiers and their corresponding attendee ranges
- **validate_booking_eligibility**: Checks if a booking request meets the minimum and maximum attendee requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **match-ticket-total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost for 50 attendees?"

**🤖 AI Agent:**
> The total cost for 50 attendees is $450.00, with a unit price of $9.00 per ticket.

---

**👤 You:**
> "Is a group of 2 people eligible for booking?"

**🤖 AI Agent:**
> No, the group is ineligible because it is too small.

---

**👤 You:**
> "How much does one ticket cost for 100 people?"

**🤖 AI Agent:**
> For 100 attendees, the unit price is $5.00 per ticket.


## ❓ FAQ

**Q: How do I calculate the total cost for my group?**
You can use the `calculate_total_cost` tool by providing the total number of attendees.

**Q: Can I check if my group size is valid?**
Yes, use the `validate_booking_eligibility` tool to verify if your group meets the minimum and maximum requirements.

**Q: How are the pricing tiers structured?**
You can view all available tiers and their attendee ranges by calling the `list_pricing_structure` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/match-ticket-total](https://vinkius.com/en/ai-agent-connect/match-ticket-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **match-ticket-total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `match-ticket-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **match-ticket-total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "match-ticket-total": {
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
