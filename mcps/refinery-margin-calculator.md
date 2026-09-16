# Refinery Margin Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/refinery-margin-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate refinery gross margins, net margins, and crack spreads.

## Description
This MCP server provides essential tools for refinery economics. It allows AI agents to calculate `calculate_gross_margin` for specific crude slates, determine the bottom-line profitability using `calculate_net_margin`, and analyze specific profitability via `calculate_crack_spread`. It also includes `optimize_slates` to identify the most profitable combination of crude grades and product yields.


## Available Tools (4)
- **calculate_crack_spread**: Calculates the crack spread for a single crude type into specific products
- **calculate_gross_margin**: Calculates the gross margin for a specific crude slate and product yield
- **calculate_net_margin**: Calculates the net margin after operating costs
- **optimize_slates**: Finds the combination of crude and products that maximizes net margin


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Refinery Margin Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the gross margin for a crude costing $70 with a 50% yield of gasoline at $100 and 50% yield of diesel at $80?"

**🤖 AI Agent:**
> The gross margin is $30.00.

---

**👤 You:**
> "Calculate the crack spread for crude at $80 with 80% gasoline at $110 and 20% diesel at $90."

**🤖 AI Agent:**
> The crack spread is $14.00.

---

**👤 You:**
> "If my gross margin is $50 and my operating costs are $20, what is my net margin?"

**🤖 AI Agent:**
> Your net margin is $30.00.


## ❓ FAQ

**Q: How do I calculate the net margin?**
You can use the `calculate_net_margin` tool by providing the gross margin data and the total operating costs.

**Q: What is a crack spread?**
A crack spread is the difference between the price of a barrel of crude oil and the value of the refined products produced from it. Use `calculate_crack_spread` to find this value.

**Q: Can I optimize my crude selection?**
Yes, the `optimize_slates` tool evaluates different crude and product combinations to find the maximum net margin.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/refinery-margin-calculator](https://vinkius.com/en/ai-agent-connect/refinery-margin-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Refinery Margin Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `refinery-margin-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Refinery Margin Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "refinery-margin-calculator": {
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
