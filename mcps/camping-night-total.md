# Camping Night Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/camping-night-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate total camping costs based on tier, nights, and region.

## Description
This MCP server provides tools to manage camping trip expenses. Use `get_tier_rates` to view pricing for different campsite tiers, `calculate_stay_cost` to determine the total price for a stay, and `validate_booking_eligibility` to check if a booking meets camping rules. It supports different regions like USA and EU.


## Available Tools (4)
- **get_tier_rates**: Retrieves the current nightly fee for all available camping tiers
- **list_available_tiers**: Provides a simple list of all tier names available in a specific region
- **validate_booking_eligibility**: Checks if a specific stay configuration is valid according to camping rules
- **calculate_stay_cost**: Calculates the total amount a camper will pay for a specific stay


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Camping Night Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much does it cost to stay 3 nights in a Tier A site in the USA?"

**🤖 AI Agent:**
> The total cost for a 3-night stay in a Tier A site in the USA is $45.00.

---

**👤 You:**
> "What are the available camping tiers in the EU?"

**🤖 AI Agent:**
> The available tiers in the EU are Tier A (Standard), Tier B (Premium), and Tier C (Luxury).

---

**👤 You:**
> "Is it possible to book a Tier B site for 10 nights in the USA?"

**🤖 AI Agent:**
> No, Tier B sites have a maximum stay limit of 7 consecutive nights.


## ❓ FAQ

**Q: How do I find out the price for a specific campsite tier?**
You can use the `get_tier_rates` tool to see the nightly fees for all available tiers in your chosen region.

**Q: Can I calculate the total cost for my entire trip?**
Yes, use the `calculate_stay_cost` tool by providing the tier name, the number of nights, and the region.

**Q: How do I know if my booking is allowed?**
Use the `validate_booking_eligibility` tool to check if your requested stay complies with regional camping rules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/camping-night-total](https://vinkius.com/en/ai-agent-connect/camping-night-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Camping Night Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `camping-night-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Camping Night Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "camping-night-total": {
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
