# WeChat Red Packet Simulator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wechat-red-packet-simulator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Simulate deterministic WeChat 'Lucky Money' distributions with inequality metrics.

## Description
This MCP server provides precise tools to simulate WeChat Red Packet (Hongbao) distributions. It implements the 'double average' constraint for fair random distributions and provides statistical analysis including the Gini coefficient to measure inequality. Use `simulate_distribution` to generate specific fund breakdowns, `get_distribution_stats` to analyze existing distributions, and `validate_constraints` to ensure a total amount can support the minimum 0.01 RMB requirement per recipient.


## Available Tools (3)
- **get_distribution_stats**: Provides high-level summary metrics for a previously generated distribution
- **simulate_distribution**: Generates a specific distribution of funds based on the chosen logic
- **validate_constraints**: 01 RMB.

Checks if a specific distribution configuration is valid under WeChat's economic rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WeChat Red Packet Simulator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Simulate a fair random distribution of 100 RMB for 10 people."

**🤖 AI Agent:**
> The distribution has been generated. The amounts are [12.45, 8.32, 15.10, 7.55, 11.20, 9.88, 13.40, 6.12, 10.50, 5.48]. The Lucky King received 15.10 RMB and the Gini coefficient is 0.24.

---

**👤 You:**
> "Divide 50 RMB equally among 5 recipients."

**🤖 AI Agent:**
> Each of the 5 recipients receives exactly 10.00 RMB.

---

**👤 You:**
> "Check if 5 RMB is enough for 600 people."

**🤖 AI Agent:**
> No, it is not possible. The required minimum is 6.00 RMB, resulting in a shortfall of 1.00 RMB.


## ❓ FAQ

**Q: What is the difference between the distribution types?**
Fixed Equal divides the total amount equally among all recipients, while Random Fair uses a probabilistic approach where each person's share is bounded by twice the current average of the remaining funds.

**Q: How is the inequality measured?**
Inequality is measured using the Gini coefficient, which ranges from 0 (perfect equality) to 1 (extreme inequality).

**Q: Can I simulate a distribution that is too small?**
If the total amount is less than 0.01 RMB multiplied by the number of recipients, the `validate_constraints` tool will flag the configuration as impossible.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wechat-red-packet-simulator](https://vinkius.com/ai-agent-connect/wechat-red-packet-simulator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WeChat Red Packet Simulator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wechat-red-packet-simulator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WeChat Red Packet Simulator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wechat-red-packet-simulator": {
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
