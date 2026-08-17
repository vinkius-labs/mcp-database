# Oracle Manipulation Detection Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/oracle-manipulation-detection-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Detect and avoid token price manipulation by analyzing oracle deviations and DEX spot prices.

## Description
This MCP server provides deterministic tools to identify and mitigate oracle price manipulation attacks. By comparing multiple oracle sources like Chainlink and Pyth against DEX spot prices, it calculates oracle deviation and identifies stale data. Use `analyze_price_integrity` to detect manipulation flags, `calculate_safe_price` to derive a consensus median price, and `get_manipulation_probability` to assess risk based on historical patterns. It helps trading systems decide whether to proceed, use caution, or halt activity to avoid losses from manipulated price feeds.


## Available Tools (3)
- **analyze_price_integrity**: Evaluates the current state of oracle and DEX prices to identify immediate manipulation risks
- **calculate_safe_price**: Derives a single reliable price from multiple oracle inputs
- **get_manipulation_probability**: Quantifies the risk of a price deviation being an attack based on historical patterns


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Oracle Manipulation Detection Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if the current oracle prices are being manipulated."

**🤖 AI Agent:**
> The current oracle deviation is 2.5%, which is within normal bounds. The trading recommendation is to proceed.

---

**👤 You:**
> "Calculate a reliable price from these oracle values: 100, 102, 98, 101."

**🤖 AI Agent:**
> The safe price is 100.5.

---

**👤 You:**
> "What is the probability that a 7% deviation is a manipulation?"

**🤖 AI Agent:**
> Based on historical data, there is an 85% probability that a 7% deviation represents a manipulation event.


## ❓ FAQ

**Q: How does the tool detect manipulation?**
The `analyze_price_integrity` tool flags manipulation when the deviation between oracles exceeds 5%, one oracle matches the DEX spot price while the other does not, and the diverging oracle is stale.

**Q: What is a safe price?**
A safe price is a consensus value, typically the median of all healthy, non-stale oracle prices, calculated using `calculate_safe_price`.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/oracle-manipulation-detection-strategy](https://vinkius.com/ai-agent-connect/oracle-manipulation-detection-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Oracle Manipulation Detection Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `oracle-manipulation-detection-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Oracle Manipulation Detection Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "oracle-manipulation-detection-strategy": {
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
