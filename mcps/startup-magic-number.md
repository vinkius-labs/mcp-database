# Startup Magic Number MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/startup-magic-number)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate SaaS sales efficiency, magic number, and payback period.

## Description
This MCP server provides essential SaaS metrics to evaluate sales and marketing efficiency. It allows AI agents to calculate the Magic Number, determine the equivalent payback period, and assess overall sales efficiency. By accounting for revenue lag and seasonality, it provides a realistic view of growth velocity. Use `get_magic_number` to find sales velocity, `get_payback_period` to estimate investment recovery, and `compare_efficiency_tiers` to categorize performance.


## Available Tools (4)
- **compare_efficiency_tiers**: Categorizes the calculated magic number into standard industry efficiency tiers
- **get_magic_number**: Calculates the core Magic Number to determine sales velocity
- **get_payback_period**: Calculates the equivalent time needed to recover sales investment
- **get_sales_efficiency**: Provides a holistic view of sales effectiveness


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Startup Magic Number** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our magic number if current revenue is $120,000, previous was $100,000, and prior sales spend was $10,000?"

**🤖 AI Agent:**
> Your magic number is 2.0.

---

**👤 You:**
> "How many months will it take to recover our sales investment for this quarter?"

**🤖 AI Agent:**
> The equivalent payback period is 6 months.

---

**👤 You:**
> "Is a magic number of 1.5 considered efficient?"

**🤖 AI Agent:**
> A magic number of 1.5 is categorized as Healthy.


## ❓ FAQ

**Q: What is the Magic Number?**
The Magic Number is a ratio that measures how much new recurring revenue is generated for every dollar spent on sales and marketing, accounting for revenue lag.

**Q: How does this tool handle revenue lag?**
The `get_magic_number` tool uses the sales spend from the prior period to account for the time it takes for sales efforts to yield actual revenue.

**Q: Can I adjust for seasonal trends?**
Yes, the `get_sales_efficiency` tool includes an optional seasonality adjustment coefficient to normalize scores against historical seasonal patterns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/startup-magic-number](https://vinkius.com/en/ai-agent-connect/startup-magic-number)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Startup Magic Number** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `startup-magic-number` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Startup Magic Number** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "startup-magic-number": {
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
