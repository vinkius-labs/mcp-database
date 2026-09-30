# Housewarming Party Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/housewarming-party-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Coordinate guest lists, catering, home readiness, and budgets for your housewarming.

## Description
This MCP server provides a complete suite of tools to manage every logistical pillar of a housewarming event. Use `get_guest_list` to track attendees and dietary needs, `calculate_catering_needs` to estimate food and drink quantities, `check_home_readiness` to assess seating and cleaning tasks, and `track_budget` to monitor your spending. It acts as a central coordination hub for domestic celebrations.


## Available Tools (4)
- **check_home_readiness**: Check if the house is ready and seating is sufficient
- **track_budget**: Track budget and expenses
- **calculate_catering_needs**: Calculate food and drink estimates
- **get_guest_list**: Get the list of guests and their requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Housewarming Party Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Who is coming to the party?"

**🤖 AI Agent:**
> The current guest list includes Alice (accepted, vegetarian), Bob (pending), and Charlie (accepted, nut allergy).

---

**👤 You:**
> "How much food should I buy for 15 guests?"

**🤖 AI Agent:**
> For 15 guests, you should prepare 15 appetizers, 15 mains, and 15 desserts, along with sufficient alcoholic and non-alcoholic beverages.

---

**👤 You:**
> "How much of my $500 budget is left?"

**🤖 AI Agent:**
> You have spent $350 so far, leaving you with $150 remaining in your budget.


## ❓ FAQ

**Q: How do I know if I have enough food for my guests?**
You can use the `calculate_catering_needs` tool by providing the number of guests to receive specific estimates for food and drinks.

**Q: Can I track dietary restrictions?**
Yes, the `get_guest_list` tool provides a list of guests including their specific dietary requirements.

**Q: How do I check if my house is ready for the party?**
Use the `check_home_readiness` tool with your seating capacity to get a readiness score and a list of pending tasks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/housewarming-party-planner](https://vinkius.com/en/ai-agent-connect/housewarming-party-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Housewarming Party Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `housewarming-party-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Housewarming Party Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "housewarming-party-planner": {
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
