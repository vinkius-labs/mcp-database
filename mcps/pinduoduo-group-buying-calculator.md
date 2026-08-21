# Pinduoduo Group-Buying Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/pinduoduo-group-buying-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate savings and social urgency for group-buying deals.

## Description
This MCP server provides deterministic tools to simulate the economics of the 'Pin' (group-buying) model. It allows AI agents to calculate individual savings, total group value, and social urgency. Use `calculate_group_economics` to find out how much money is saved per person, `calculate_urgency_score` to determine how close a group is to completion, and `calculate_time_to_completion` to check deal expiration.


## Available Tools (3)
- **calculate_group_economics**: Calculate individual and total group savings and members needed
- **calculate_time_to_completion**: Calculate time remaining until the group deal expires
- **calculate_urgency_score**: Calculate the social urgency score of a group


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pinduoduo Group-Buying Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will I save if the base price is 100 RMB, the group price is 70 RMB, and we need 5 people total?"

**🤖 AI Agent:**
> You will save 30 RMB per person, and the total group savings will be 150 RMB for the 5 members.

---

**👤 You:**
> "The group needs 10 people and currently has 9. How urgent is this?"

**🤖 AI Agent:**
> The urgency score is 100, meaning only one more person is needed to unlock the discount.

---

**👤 You:**
> "Is the deal still active if there are 0 minutes remaining?"

**🤖 AI Agent:**
> No, the deal is considered expired.


## ❓ FAQ

**Q: What does the urgency score represent?**
The urgency score is a metric from 0 to 100. A score of 100 means the group is exactly one person away from reaching the required threshold to unlock the discount.

**Q: How is individual savings calculated?**
Individual savings is the difference between the `itemBasePriceRmb` and the `groupDiscountPriceRmb` provided to the `calculate_group_economics` tool.

**Q: Can I use this to track deal expiration?**
Yes, you can use the `calculate_time_to_completion` tool to check if a group deal is still active or has expired.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/pinduoduo-group-buying-calculator](https://vinkius.com/ai-agent-connect/pinduoduo-group-buying-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pinduoduo Group-Buying Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pinduoduo-group-buying-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pinduoduo Group-Buying Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pinduoduo-group-buying-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
