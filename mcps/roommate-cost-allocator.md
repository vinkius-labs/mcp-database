# Roommate Cost Allocator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/roommate-cost-allocator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Fairly distribute rent, utilities, and parking costs among roommates.

## Description
This MCP server provides tools to calculate fair rent splits based on private room size, amenities, and parking usage. Use `calculate_rent_split` to determine individual monthly obligations, `get_area_distribution_summary` to view space allocation, `simulate_amenity_impact` to model changes in amenity status, and `validate_cost_integrity` to ensure all shares sum correctly to the total household cost.


## Available Tools (4)
- **calculate_rent_split**: Calculates the individual financial obligations for each roommate based on their specific living conditions
- **get_area_distribution_summary**: Provides a high-level overview of how living space is distributed among the household
- **simulate_amenity_impact**: Allows roommates to see how much the total cost would change if someone gained or lost a private amenity
- **validate_cost_integrity**: Verifies that the sum of all individual shares perfectly matches the total household cost


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Roommate Cost Allocator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the rent split for 3 roommates: Alice (200 sqft, has amenity, no parking), Bob (150 sqft, no amenity, has parking), and Charlie (150 sqft, no amenity, no parking). Total rent is 3000, utilities are 300, parking is 100 per space, and amenity premium is 100."

**🤖 AI Agent:**
> Alice: $1,233.33, Bob: $1,133.33, Charlie: $1,033.33.

---

**👤 You:**
> "Show me the area distribution for roommates Alice (200 sqft), Bob (150 sqft), and Charlie (150 sqft)."

**🤖 AI Agent:**
> Total private area is 500 sqft. Alice: 40%, Bob: 30%, Charlie: 30%.

---

**👤 You:**
> "What happens to the rent if Bob gets a private amenity? Current setup: Alice (200 sqft, amenity), Bob (150 sqft, no amenity), Charlie (150 sqft, no amenity). Rent 3000, utilities 300, amenity premium 100."

**🤖 AI Agent:**
> The total cost remains the same, but Bob's share increases by the amenity premium while others' shares decrease proportionally.


## ❓ FAQ

**Q: How is the rent split calculated?**
The split uses `calculate_rent_split` to weigh costs based on private square footage, adding premiums for amenities and specific costs for parking.

**Q: Can I see how a new balcony would affect the rent?**
Yes, you can use `simulate_amenity_impact` to see how adding or removing a private amenity changes the total cost and individual shares.

**Q: How do I know if the math is correct?**
You can run `validate_cost_integrity` to verify that the sum of all individual shares matches the total expected household cost.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/roommate-cost-allocator](https://vinkius.com/en/ai-agent-connect/roommate-cost-allocator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Roommate Cost Allocator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `roommate-cost-allocator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Roommate Cost Allocator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "roommate-cost-allocator": {
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
