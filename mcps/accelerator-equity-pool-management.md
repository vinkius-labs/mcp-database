# Accelerator Equity Pool Management MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-equity-pool-management)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Manage and forecast accelerator equity allocation, utilization, and runway.

## Description
This MCP server provides tools to manage the lifecycle of an accelerator's equity pool. It allows for real-time monitoring of pool health using `get_pool_status`, projecting future capacity with `forecast_runway`, and determining necessary liquidity through `calculate_replenishment_needs`. It helps managers track equity tiers from reserved to recycled, ensuring the program maintains sufficient runway for future cohorts.


## Available Tools (3)
- **calculate_replenishment_needs**: Determines how much equity must be recovered through exits or secondary sales to maintain a specific operational target
- **forecast_runway**: Answers how many future cohorts the accelerator can sustain with current resources
- **get_pool_status**: Provides a high-level snapshot of the current health and availability of the equity pool


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Equity Pool Management** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current status of my equity pool if I have 10% total, 2% reserved, and 5% committed?"

**🤖 AI Agent:**
> Your current utilization rate is 62.5%, and you have 3% of available equity remaining.

---

**👤 You:**
> "How many more cohorts can I run if I have 5% available equity, 2 companies per cohort, and take 2% per company?"

**🤖 AI Agent:**
> You can support 2 more full cohorts.

---

**👤 You:**
> "I have 1% available equity and want a 3% buffer. How much do I need to replenish?"

**🤖 AI Agent:**
> You have a shortfall of 2% to reach your target buffer.


## ❓ FAQ

**Q: How can I check if my equity pool is running low?**
You can use the `get_pool_status` tool to see your current utilization rate and the amount of available equity remaining.

**Q: How do I know how many more cohorts I can support?**
The `forecast_runway` tool calculates exactly how many future cohorts and years of operation are possible based on your current equity and cohort structure.

**Q: What should I do if my available equity falls below my target buffer?**
Use `calculate_replenishment_needs` to determine the exact shortfall and the volume of secondary sales required to restore your target safety margin.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-equity-pool-management](https://vinkius.com/ai-agent-connect/accelerator-equity-pool-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Equity Pool Management** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-equity-pool-management` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Equity Pool Management** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-equity-pool-management": {
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
