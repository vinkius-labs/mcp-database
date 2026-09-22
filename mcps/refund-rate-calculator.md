# Refund Rate Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/refund-rate-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze e-commerce refund metrics, including monetary rates and volume impact.

## Description
This MCP server provides essential tools for e-commerce analysis by calculating key refund performance indicators. Use `get_refund_rate` to determine the monetary impact of returns, `get_volume_refund_rate` to see how many orders were affected, or `compare_refund_metrics` for a complete overview of revenue loss versus order frequency. It connects your AI agent to transaction and refund data tiers to provide instant insights into product quality and customer satisfaction.


## Available Tools (4)
- **compare_refund_metrics**: Provides a comprehensive summary comparing monetary impact versus volume impact
- **get_net_revenue**: Determines the actual revenue retained after accounting for refunds
- **get_refund_rate**: Calculates the monetary refund rate for a specific set of orders
- **get_volume_refund_rate**: Calculates the frequency of refunds based on the number of orders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Refund Rate Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the monetary refund rate for orders ORD-101 and ORD-102?"

**🤖 AI Agent:**
> The monetary refund rate for those orders is 15.5%, with a total order value of $200.00 and total refunds of $31.00.

---

**👤 You:**
> "How many orders were affected by refunds in this batch: ORD-201, ORD-202, ORD-203?"

**🤖 AI Agent:**
> Out of the 3 orders analyzed, 1 order resulted in a refund, representing a volume refund rate of 33.33%.

---

**👤 You:**
> "Compare the monetary and volume impact for orders ORD-301 through ORD-305."

**🤖 AI Agent:**
> The monetary rate is 5.0% and the volume rate is 20.0%, resulting in a total revenue impact of $25.00.


## ❓ FAQ

**Q: What is the difference between monetary and volume refund rates?**
The monetary rate measures the percentage of total revenue lost to refunds, while the volume rate measures the percentage of total orders that resulted in a refund.

**Q: How can I see the total revenue remaining after refunds?**
You can use the `get_net_revenue` tool to calculate the actual revenue retained after subtracting all refund amounts from the total order values.

**Q: Which AI clients can use this tool?**
This tool is compatible with Cursor, VS Code, Claude Desktop, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/refund-rate-calculator](https://vinkius.com/en/ai-agent-connect/refund-rate-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Refund Rate Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `refund-rate-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Refund Rate Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "refund-rate-calculator": {
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
