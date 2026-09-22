# Yarn Ball Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/yarn-ball-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [planning](../categories/planning.md)

Calculate required yarn balls and project costs for textile crafts.

## Description
This MCP server provides essential tools for textile and craft planning. Use `get_required_balls` to determine how many whole units to purchase, `validate_supply_sufficiency` to check your current stock against project needs, `calculate_project_cost_estimate` to budget for materials, and `get_yarn_inventory_summary` to see your total available length. It ensures you never run out of material mid-project by rounding up to the nearest whole ball.


## Available Tools (4)
- **get_required_balls**: Calculates the total number of yarn balls a user must purchase to meet their total requirement
- **get_yarn_inventory_summary**: Provides a summary of the total length of yarn available based on a current inventory count
- **validate_supply_sufficiency**: Determines if a user's current inventory of yarn balls is enough to complete a specific project
- **calculate_project_cost_estimate**: Estimates the total cost of purchasing the necessary yarn for a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Yarn Ball Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many 50m balls of yarn do I need for a project that requires 125m?"

**🤖 AI Agent:**
> You will need 3 balls of yarn.

---

**👤 You:**
> "I have 2 balls of 100m yarn. Is that enough for a 250m project?"

**🤖 AI Agent:**
> No, your supply is insufficient. You need 1 more ball.

---

**👤 You:**
> "What is the total cost if I need 5 balls of yarn and each ball costs $4.50?"

**🤖 AI Agent:**
> The total estimated cost is $22.50.


## ❓ FAQ

**Q: How does the tool handle partial balls of yarn?**
The `get_required_balls` tool always rounds up to the next whole number, ensuring you have enough yarn to complete your project.

**Q: Can I check if I have enough yarn in my current stash?**
Yes, you can use `validate_supply_sufficiency` to compare your current ball count against the total length required for a project.

**Q: How is the project cost calculated?**
The `calculate_project_cost_estimate` tool calculates the total cost by multiplying the number of whole balls needed by the price per ball.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/yarn-ball-calculator](https://vinkius.com/en/ai-agent-connect/yarn-ball-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Yarn Ball Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `yarn-ball-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Yarn Ball Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "yarn-ball-calculator": {
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
