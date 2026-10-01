# Food Donation Allocation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/food-donation-allocation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Optimizes the distribution of surplus food to recipient groups based on dietary needs and transport limits.

## Description
This MCP server acts as a logistics engine to minimize food waste. It connects AI agents to surplus food inventories and recipient organizations. Using `query_available_surplus`, agents can identify available food items. The `find_eligible_recipients` tool identifies groups that meet specific dietary requirements. For logistics planning, `calculate_optimal_allocation` generates distribution plans that respect transport limits and expiry priority, while `validate_allocation_feasibility` ensures proposed plans are physically and dietarily possible.


## Available Tools (4)
- **calculate_optimal_allocation**: Generates a suggested plan to distribute food to recipients based on priority and constraints
- **find_eligible_recipients**: Finds groups capable of receiving specific types of food
- **query_available_surplus**: Identifies all currently available food supplies that have not yet been allocated
- **validate_allocation_feasibility**: Checks if a specific proposed allocation plan is physically and dietarily possible


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Food Donation Allocation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What surplus food is currently available that is vegan?"

**🤖 AI Agent:**
> The available vegan surplus includes 50 portions of organic lentils and 30 portions of quinoa.

---

**👤 You:**
> "Find recipient groups that can accept gluten-free food."

**🤖 AI Agent:**
> The eligible recipient groups are Community Kitchen Alpha and the City Food Bank.

---

**👤 You:**
> "Create an allocation plan for these food IDs: food_1, food_2 with a transport limit of 100 portions."

**🤖 AI Agent:**
> The optimal allocation plan distributes 60 portions of food_1 to Recipient_A and 40 portions of food_2 to Recipient_B, utilizing the full 100 portion transport capacity.


## ❓ FAQ

**Q: How does the tool handle food expiration?**
The `calculate_optimal_allocation` tool prioritizes items with the earliest expiration dates to ensure food is distributed before it spoils.

**Q: Can I filter food by dietary requirements?**
Yes, you can use `query_available_surplus` with a dietary filter or use `find_eligible_recipients` to find groups that match specific dietary tags.

**Q: How are transport constraints managed?**
The `transportLimit` parameter in `calculate_optimal_allocation` ensures that the total portions allocated do not exceed the available transport capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/food-donation-allocation](https://vinkius.com/en/ai-agent-connect/food-donation-allocation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Food Donation Allocation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `food-donation-allocation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Food Donation Allocation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "food-donation-allocation": {
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
