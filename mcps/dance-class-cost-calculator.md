# Dance Class Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/dance-class-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate precise tuition totals and session breakdowns for dance studios.

## Description
This MCP server provides specialized tools for dance studio management to calculate student costs. It handles individual session pricing, total tuition calculations with package discounts, billing tier eligibility checks, and detailed cost breakdowns. Use `calculate_total_tuition` to determine final amounts after discounts, or `get_session_breakdown` to see the impact of savings per class.


## Available Tools (4)
- **calculate_total_tuition**: Calculate the total amount a student owes for a specific number of sessions, considering potential package discounts
- **get_session_breakdown**: Provide a granular view of costs, showing the cost per session before and after package considerations
- **get_single_session_cost**: Determine the cost of attending exactly one dance class without any package benefits
- **verify_billing_tier_eligibility**: Check if a specific session count qualifies for a specific billing tier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dance Class Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will it cost for 10 sessions if the base rate is $20 and there is a $15 discount for 5 or more sessions?"

**🤖 AI Agent:**
> The total cost for 10 sessions is $185.00, with a $15.00 discount applied.

---

**👤 You:**
> "What is the cost of a single session with a base rate of $25?"

**🤖 AI Agent:**
> The cost for a single session is $25.00.

---

**👤 You:**
> "Show me the breakdown for 12 sessions at $30 each, with a $20 discount for 10+ sessions."

**🤖 AI Agent:**
> The original price per session was $30.00, and the final price per session is $28.33, resulting in total savings of $20.00.


## ❓ FAQ

**Q: How do I calculate the total cost for a student?**
You can use the `calculate_total_tuition` tool by providing the session count, base rate, and any applicable package discounts.

**Q: Can I check if a student qualifies for a monthly discount?**
Yes, use the `verify_billing_tier_eligibility` tool to check if a specific session count meets the requirements for tiers like 'Monthly'.

**Q: What is the cost of a single class?**
Use the `get_single_session_cost` tool with the standard base rate to find the cost of one session.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/dance-class-cost-calculator](https://vinkius.com/en/ai-agent-connect/dance-class-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dance Class Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dance-class-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dance Class Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dance-class-cost-calculator": {
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
