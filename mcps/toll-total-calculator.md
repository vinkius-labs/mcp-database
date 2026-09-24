# Toll Total Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/toll-total-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Aggregates and analyzes toll charges to calculate total travel costs.

## Description
This MCP server provides specialized tools for managing and analyzing toll expenses. It allows AI agents to calculate the sum of multiple charges using `get_total_toll_cost`, verify individual entries with `validate_toll_entry`, generate detailed breakdowns via `get_toll_summary`, and isolate expensive fees using `filter_high_value_tolls`. It is designed to help travelers and logistics planners manage cumulative transit costs accurately.


## Available Tools (4)
- **filter_high_value_tolls**: Identifies all charges that exceed a specific monetary threshold
- **get_toll_summary**: Provides a high-level breakdown of a collection of tolls
- **validate_toll_entry**: Verifies if a specific toll charge is valid
- **get_total_toll_cost**: Calculates the sum of all provided toll charges


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Toll Total Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total of these toll charges: 5.50, 12.00, and 3.25?"

**🤖 AI Agent:**
> The total toll cost is 20.75.

---

**👤 You:**
> "Show me the summary for tolls costing 10.00, 25.00, and 15.00."

**🤖 AI Agent:**
> The total amount is 50.00, with an average charge of 16.67, a maximum charge of 25.00, and a minimum charge of 10.00.

---

**👤 You:**
> "Which of these tolls are higher than 20.00: 5.00, 25.00, 10.00, and 30.00?"

**🤖 AI Agent:**
> The high value charges are 25.00 and 30.00.


## ❓ FAQ

**Q: How do I calculate the total cost of my trip?**
You can use the `get_total_toll_cost` tool by providing a list of all your individual toll amounts.

**Q: Can I check if a specific toll amount is valid?**
Yes, the `validate_toll_entry` tool checks if a toll amount is a positive, valid number.

**Q: How can I see a summary of my expenses?**
The `get_toll_summary` tool provides the total sum, average charge, and the maximum and minimum values from your list of tolls.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/toll-total-calculator](https://vinkius.com/en/ai-agent-connect/toll-total-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Toll Total Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `toll-total-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Toll Total Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "toll-total-calculator": {
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
