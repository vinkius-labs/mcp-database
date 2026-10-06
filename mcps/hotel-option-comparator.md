# Hotel Option Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hotel-option-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Ranks hotel options by cost, location, capacity, and amenities.

## Description
This MCP server provides a multi-criteria decision engine to compare hotel stays. It uses `rank_hotel_options` to prioritize hotels based on user-defined weights for cost, location, and flexibility. You can also use `calculate_stay_economics` to see detailed price breakdowns, `evaluate_policy_flexibility` to assess cancellation risks, and `get_hotel_amenities_summary` to check for breakfast and room capacity.


## Available Tools (4)
- **get_hotel_amenities_summary**: Retrieves a quick snapshot of the room's capacity and breakfast availability
- **calculate_stay_economics**: Analyzes the financial breakdown of a specific hotel option
- **evaluate_policy_flexibility**: Quantifies the risk level associated with a hotel's cancellation policy
- **rank_hotel_options**: Ranks supplied hotels by total stay cost, location score, room capacity, breakfast, fees, cancellation terms, and user weights


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hotel Option Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare these hotels: H1, H2, H3 for 2 guests and 3 nights. I care most about low cost and location."

**🤖 AI Agent:**
> Hotel H2 is the best option with a score of 85, costing $300 total, while Hotel H1 costs $350.

---

**👤 You:**
> "What is the total cost for staying at hotel H1 for 4 nights?"

**🤖 AI Agent:**
> The total stay cost for hotel H1 for 4 nights is $420, including $380 base rate and $40 in fees.

---

**👤 You:**
> "How flexible is the cancellation policy for hotel H2?"

**🤖 AI Agent:**
> Hotel H2 offers a highly flexible policy that allows you to cancel anytime without penalty.


## ❓ FAQ

**Q: How does the ranking work?**
The `rank_hotel_options` tool calculates a score by normalizing dimensions like cost and location, then applying your specific preference weights.

**Q: Can I see the total price including taxes?**
Yes, use `calculate_stay_economics` to get the full breakdown of base rates, service fees, and total stay cost.

**Q: How do I check if breakfast is included?**
You can use `get_hotel_amenities_summary` to quickly check breakfast availability and room capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hotel-option-comparator](https://vinkius.com/en/ai-agent-connect/hotel-option-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hotel Option Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hotel-option-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hotel Option Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hotel-option-comparator": {
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
