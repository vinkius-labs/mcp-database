# Restaurant Cover Charge Manager MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/restaurant-cover-charge-manager)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate and manage restaurant cover charges and revenue projections.

## Description
This MCP server provides tools for restaurant management to handle cover charges. Use `calculate_total_cover` to determine the total fee for a party, `get_tiered_rate` to find per-person rates based on group size, `validate_party_eligibility` to check if a group meets minimum size requirements, and `summarize_revenue_projection` to estimate total income from expected guests.


## Available Tools (4)
- **calculate_total_cover**: Calculates the total cover charge for a specific party
- **get_tiered_rate**: Determines the applicable charge per guest based on the size of the party
- **summarize_revenue_projection**: Estimates total expected revenue from cover charges
- **validate_party_eligibility**: Checks if a party meets the specific requirements to be charged a cover


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Restaurant Cover Charge Manager** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cover charge for 10 guests at $5 each?"

**🤖 AI Agent:**
> The total cover charge for 10 guests at $5 each is $50.00.

---

**👤 You:**
> "Is a party of 3 eligible if the minimum size is 5?"

**🤖 AI Agent:**
> No, the party is not eligible because the guest count is below the minimum requirement of 5.

---

**👤 You:**
> "What is the rate for a group of 20 people?"

**🤖 AI Agent:**
> The applicable rate for a group of 20 people is $4.00 per guest.


## ❓ FAQ

**Q: How do I calculate the total fee for a large group?**
You can use the `calculate_total_cover` tool by providing the guest count and the charge per guest.

**Q: Can I check if a group is large enough for a cover charge?**
Yes, use `validate_party_eligibility` to check if the guest count meets your minimum requirements.

**Q: How can I estimate my event revenue?**
Use `summarize_revenue_projection` with the expected guest count and the rate per guest.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/restaurant-cover-charge-manager](https://vinkius.com/en/ai-agent-connect/restaurant-cover-charge-manager)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Restaurant Cover Charge Manager** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `restaurant-cover-charge-manager` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Restaurant Cover Charge Manager** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "restaurant-cover-charge-manager": {
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
