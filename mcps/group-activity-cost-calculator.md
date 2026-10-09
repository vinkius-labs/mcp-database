# Group Activity Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/group-activity-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate total group expenses and individual splits for activities.

## Description
This MCP server provides precise financial tools for planning group activities. It allows AI agents to determine total costs, verify if individual splits match the group total, generate pricing summaries, and estimate how many people can join based on a fixed budget. Use `calculate_total_cost` to find the total amount needed, or `estimate_budget_limit` to see how many participants a specific budget can cover.


## Available Tools (4)
- **calculate_total_cost**: Determines the total amount of money needed for the entire group
- **estimate_budget_limit**: Determines how many people can participate given a strict maximum budget
- **get_group_pricing_summary**: Provides a high-level breakdown of the financial requirements for a group
- **verify_split_consistency**: Validates that a proposed total cost matches the sum of individual contributions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Group Activity Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost for 15 people if each person pays $25?"

**🤖 AI Agent:**
> The total cost for 15 people at $25 each is $375.

---

**👤 You:**
> "How many people can join if I have a budget of $500 and the price is $40 per person?"

**🤖 AI Agent:**
> With a budget of $500 and a unit price of $40, a maximum of 12 people can participate.

---

**👤 You:**
> "Give me a summary for 10 people at $15 per person."

**🤖 AI Agent:**
> For 10 participants at $15 each, the total cost is $150.


## ❓ FAQ

**Q: How do I calculate the total cost for my group?**
You can use the `calculate_total_cost` tool by providing the number of participants and the price per person.

**Q: Can I check if my budget is sufficient for a specific number of people?**
Yes, use the `estimate_budget_limit` tool to find out the maximum number of participants your budget can accommodate.

**Q: How can I verify if the total amount collected is correct?**
The `verify_split_consistency` tool validates that the proposed total matches the sum of individual contributions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/group-activity-cost-calculator](https://vinkius.com/en/ai-agent-connect/group-activity-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Group Activity Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `group-activity-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Group Activity Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "group-activity-cost-calculator": {
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
