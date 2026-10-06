# Group Room Cost Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/group-room-cost-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A precision engine for splitting lodging expenses by occupancy, room type, and privacy.

## Description
This MCP server provides a weighted allocation model to split lodging costs fairly among group members. It accounts for occupancy duration, room type value, bed privacy, and proportional distribution of shared fees and taxes. Use `generate_cost_split` to calculate final amounts, `get_room_rate_tiers` to find valid room categories, and `validate_stay_details` to ensure stay configurations are logically consistent.


## Available Tools (4)
- **generate_cost_split**: Produces a finalized list of what each person owes
- **validate_stay_details**: Validates a proposed group stay configuration
- **calculate_individual_weight**: Calculates a single person's relative cost weight
- **get_room_rate_tiers**: Retrieves available room categories and base prices for a region


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Group Room Cost Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the cost split for 3 people staying 2 nights in a Standard room. Total fees are 50 and taxes are 30. Member A has a private bed, while B and C share a bed."

**🤖 AI Agent:**
> Member A owes 120.00, Member B owes 80.00, and Member C owes 80.00.

---

**👤 You:**
> "What are the available room tiers for the USA region?"

**🤖 AI Agent:**
> The available tiers for the USA are Standard ($100), Premium ($200), and Luxury ($400).

---

**👤 You:**
> "Check if this stay configuration is valid: 2 members, one in a Suite and one in a Standard room."

**🤖 AI Agent:**
> The stay configuration is valid.


## ❓ FAQ

**Q: How does the tool calculate the final amount owed?**
The engine calculates an individual weight based on nights stayed, room type, and bed privacy, then distributes the total cost (including fees and taxes) proportionally based on those weights.

**Q: Can I adjust the split for specific people?**
Yes, you can use the `customWeightMultiplier` within the weight calculation to adjust an individual's share based on pre-agreed social factors.

**Q: How do I know which room types are available?**
You can use the `get_room_rate_tiers` tool to retrieve the available room categories and their base price levels for a specific region.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/group-room-cost-splitter](https://vinkius.com/en/ai-agent-connect/group-room-cost-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Group Room Cost Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `group-room-cost-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Group Room Cost Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "group-room-cost-splitter": {
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
