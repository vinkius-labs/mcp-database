# Souvenir Budget Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/souvenir-budget-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Intelligent budget allocation for souvenirs based on recipient priority, customs laws, and luggage space.

## Description
This MCP server provides a specialized engine for travelers to manage souvenir spending. It uses `get_recipient_priority_weights` to distribute funds based on how important each recipient is, `validate_customs_compliance` to ensure you stay within duty-free limits, and `calculate_luggage_utilization` to prevent overpacking. Finally, `generate_optimized_allocation` calculates the exact amount to spend per person to maximize your budget efficiency.


## Available Tools (4)
- **calculate_luggage_utilization**: Calculates how much physical space the planned souvenirs will occupy
- **generate_optimized_allocation**: Distributes the total budget across recipients based on priorities
- **get_recipient_priority_weights**: Determines the proportional weight of each recipient based on their priority level
- **validate_customs_compliance**: Checks if the proposed spending per destination adheres to regional customs laws


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Souvenir Budget Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a $500 budget. I want to buy gifts for Mom (Priority 5) and a Friend (Priority 2). How much should I spend on each?"

**🤖 AI Agent:**
> Based on the priority weights, you should allocate $384.62 to Mom and $115.38 to your Friend.

---

**👤 You:**
> "I'm planning to spend $600 in France. Will I hit customs limits?"

**🤖 AI Agent:**
> Your planned spending of $600 exceeds the duty-free limit for France by $100.

---

**👤 You:**
> "I have 20 liters of space. I want to buy 5 magnets (0.5L each) and 2 figurines (4L each). Do they fit?"

**🤖 AI Agent:**
> Yes, the total volume is 10.5 liters, leaving you with 9.5 liters of remaining space.


## ❓ FAQ

**Q: How does the budget distribution work?**
The budget is distributed using a weighted system. By using `generate_optimized_allocation`, the tool assigns more funds to recipients with higher priority levels.

**Q: Can I check if my souvenirs will fit in my suitcase?**
Yes, the `calculate_luggage_utilization` tool calculates the total volume of your planned items against your available capacity.

**Q: Will this help me avoid customs issues?**
Yes, `validate_customs_compliance` checks your planned spending against known duty-free thresholds for various destinations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/souvenir-budget-planner](https://vinkius.com/en/ai-agent-connect/souvenir-budget-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Souvenir Budget Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `souvenir-budget-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Souvenir Budget Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "souvenir-budget-planner": {
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
