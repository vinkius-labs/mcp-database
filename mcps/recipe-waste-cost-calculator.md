# Recipe Waste Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/recipe-waste-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate financial loss from food waste in recipe batches.

## Description
This MCP server provides tools to quantify the financial impact of food waste. Use `get_waste_impact` to find the monetary loss for a single batch, `get_batch_waste_summary` to aggregate waste across multiple batches, `categorize_waste_severity` to determine business priority, and `compare_waste_scenarios` to evaluate different waste outcomes.


## Available Tools (4)
- **categorize_waste_severity**: Determines the business priority level for a specific waste event
- **compare_waste_scenarios**: Compares two different waste outcomes to see the difference in financial impact
- **get_batch_waste_summary**: Provides a high-level overview of waste across multiple batch scenarios
- **get_waste_impact**: Calculates the specific monetary loss for a single recipe batch


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recipe Waste Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the wasted cost for a batch that costs $500 with a 10% waste percentage?"

**🤖 AI Agent:**
> The wasted cost for this batch is $50.00.

---

**👤 You:**
> "Summarize the waste for batches costing $100, $200, and $300 with waste percentages of 5%, 10%, and 15%."

**🤖 AI Agent:**
> The total waste cost is $60.00, with an average waste percentage of 10% across 3 batches.

---

**👤 You:**
> "Is a 25% waste percentage considered serious?"

**🤖 AI Agent:**
> A 25% waste percentage is categorized as High severity, requiring immediate intervention.


## ❓ FAQ

**Q: How do I calculate the loss for one specific batch?**
You can use the `get_waste_impact` tool by providing the total batch cost and the waste percentage.

**Q: Can I compare two different waste scenarios?**
Yes, the `compare_waste_scenarios` tool allows you to compare two scenarios to see the difference in financial impact.

**Q: How is waste severity determined?**
The `categorize_waste_severity` tool classifies waste into levels like Low, Medium, or High to help prioritize business responses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/recipe-waste-cost-calculator](https://vinkius.com/en/ai-agent-connect/recipe-waste-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Recipe Waste Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `recipe-waste-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Recipe Waste Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recipe-waste-cost-calculator": {
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
