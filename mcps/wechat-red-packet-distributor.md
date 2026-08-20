# WeChat Red Packet Distributor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wechat-red-packet-distributor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate fair and deterministic WeChat Red Packet distributions.

## Description
This MCP server provides precise mathematical models for distributing WeChat Red Packets (Hongbao). It allows AI agents to calculate exact monetary allocations using three distinct strategies: `fixed` for equal splits, `random_fair` using a stick-breaking algorithm to ensure fairness, and `lucky_king` for high-variance distributions. Use `validate_hongbao_config` to ensure the total amount is sufficient for the number of recipients before calculating, and `get_distribution_statistics` to analyze the resulting spread, average, and the highest amount (Lucky King).


## Available Tools (3)
- **calculate_distribution**: Generates the specific list of monetary amounts for each participant based on the selected strategy
- **get_distribution_statistics**: Analyzes a generated list of amounts to provide insight into the fairness and volatility of the distribution
- **validate_hongbao_config**: Checks if a proposed distribution scenario is mathematically possible before attempting calculation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WeChat Red Packet Distributor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you distribute 100 RMB among 10 people using the random_fair mode?"

**🤖 AI Agent:**
> The distribution for 100 RMB among 10 people using random_fair is: [12.45, 8.32, 15.10, 7.55, 11.20, 9.45, 13.08, 6.25, 10.50, 6.10].

---

**👤 You:**
> "Split 50 RMB equally between 5 people."

**🤖 AI Agent:**
> The fixed distribution for 50 RMB among 5 people is: [10.0, 10.0, 10.0, 10.0, 10.0].

---

**👤 You:**
> "Is it possible to distribute 0.05 RMB to 10 people?"

**🤖 AI Agent:**
> No, it is not possible. The minimum required amount for 10 people is 0.10 RMB.


## ❓ FAQ

**Q: What is the minimum amount required for a distribution?**
Each recipient must receive at least 0.01 RMB. You can use `validate_hongbao_config` to check if your total amount is sufficient for your group size.

**Q: How does the 'random_fair' mode work?**
The `random_fair` mode uses a stick-breaking algorithm. It ensures every person gets at least 0.01 RMB and prevents extreme inequality by capping any single person's share at twice the current remaining average.

**Q: Can I see the statistical spread of the red packet?**
Yes, after generating a distribution with `calculate_distribution`, you can pass the resulting amounts to `get_distribution_statistics` to find the average, variance, and the Lucky King amount.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wechat-red-packet-distributor](https://vinkius.com/ai-agent-connect/wechat-red-packet-distributor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WeChat Red Packet Distributor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wechat-red-packet-distributor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WeChat Red Packet Distributor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wechat-red-packet-distributor": {
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
