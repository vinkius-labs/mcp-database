# Supply Chain Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/supply-chain-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate SCM cost ratio, category breakdown, and industry benchmarks.

## Description
This MCP server provides specialized tools to measure supply chain efficiency. Use `calculate_scm_ratio` to determine total expenditure as a percentage of revenue, `get_cost_distribution` for a granular breakdown across transportation, warehousing, inventory, order processing, and administration, and `evaluate_sector_performance` to compare your results against industry benchmarks like Retail, Manufacturing, or Distribution.


## Available Tools (3)
- **get_cost_distribution**: Analyzes how the total SCM expenditure is distributed across different operational pillars
- **calculate_scm_ratio**: Calculates total SCM cost as a percentage of revenue
- **evaluate_sector_performance**: Identifies if the SCM ratio is within target and flags reduction opportunities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Supply Chain Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my SCM cost ratio if my revenue is 1000000 and total costs are 120000?"

**🤖 AI Agent:**
> Your SCM cost ratio is 12.0%.

---

**👤 You:**
> "Analyze my costs: transportation 50k, warehousing 30k, inventory 20k, order processing 10k, and administration 10k."

**🤖 AI Agent:**
> The cost distribution is: transportation 41.67%, warehousing 25.0%, inventory 16.67%, order processing 8.33%, and administration 8.33%.

---

**👤 You:**
> "Is my manufacturing sector performance good with a 9% SCM ratio?"

**🤖 AI Agent:**
> No, the target range for Manufacturing is 5% to 8%. Your current ratio of 9% exceeds the benchmark.


## ❓ FAQ

**Q: What metrics does this server calculate?**
It calculates the SCM cost ratio, provides a breakdown of costs by category using `get_cost_distribution`, and evaluates performance against industry benchmarks.

**Q: How do I identify cost reduction opportunities?**
Use the `evaluate_sector_performance` tool. It compares your current costs against sector-specific targets and flags categories that are exceeding their expected weight.

**Q: Which industries are supported for benchmarking?**
The server includes hardcoded benchmarks for Retail, Manufacturing, and Distribution sectors.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/supply-chain-cost-calculator](https://vinkius.com/mcp/supply-chain-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Supply Chain Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `supply-chain-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Supply Chain Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "supply-chain-cost-calculator": {
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
