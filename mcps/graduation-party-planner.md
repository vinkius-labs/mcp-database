# Graduation Party Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/graduation-party-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Orchestrate perfect graduation celebrations with tools for budgeting, guest lists, and timelines.

## Description
This MCP server provides a complete suite of tools to manage every aspect of a graduation celebration. You can use `create_party_profile` to set your budget and venue capacity, `plan_item` to track costs for food and decor, `manage_guest_list` to monitor invitees, and `build_timeline` to organize the event flow. It ensures your celebration stays within budget and within venue limits.


## Available Tools (5)
- **build_timeline**: Constructs the chronological flow of the event
- **manage_guest_list**: Tracks and validates the number of invitees
- **plan_item**: Adds a specific requirement to the party plan
- **create_party_profile**: Establishes the foundational constraints of the graduation event
- **get_budget_summary**: Provides a breakdown of spending across all planning pillars


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Graduation Party Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to plan a graduation party for Alex with a budget of $2000 and a venue capacity of 50 people on June 15th, 2025."

**🤖 AI Agent:**
> I have created the party profile for Alex's graduation with a $2,000 budget and a capacity for 50 guests for June 15th, 2025.

---

**👤 You:**
> "Add a catering service to Alex's party for $500."

**🤖 AI Agent:**
> Catering has been added to the plan for $500. Your remaining budget is $1,500.

---

**👤 You:**
> "What is the current status of my budget for Alex's party?"

**🤖 AI Agent:**
> You have spent $500 so far, leaving $1,500 remaining in your budget.


## ❓ FAQ

**Q: How do I set a budget limit?**
Use the `create_party_profile` tool to define your `budgetLimit` at the start of your planning session.

**Q: Can I track my spending by category?**
Yes, you can use `get_budget_summary` to see a detailed breakdown of spending across all planning pillars.

**Q: How does the tool handle venue capacity?**
When you use `manage_guest_list`, the tool checks the total number of guests against the `venueCapacity` set in your party profile to prevent overbooking.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/graduation-party-planner](https://vinkius.com/en/ai-agent-connect/graduation-party-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Graduation Party Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `graduation-party-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Graduation Party Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "graduation-party-planner": {
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
