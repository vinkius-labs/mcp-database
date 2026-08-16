# Max Pain Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/max-pain-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Determine the exact strike price that minimizes total loss for all option holders and assess pin risk.

## Description
This MCP server provides precise tools for options traders to identify the Max Pain point. By analyzing strike prices and open interest for both calls and puts, the `calculate_max_pain` tool finds the specific strike where the aggregate loss for option holders is minimized. It also identifies pin risk, which occurs when the underlying price is within 1% of the max pain strike near expiration. Use `validate_market_data` to ensure your options data is consistent and `get_strike_loss_breakdown` to see the specific call and put losses contributing to the total at any given strike.


## Available Tools (3)
- **calculate_max_pain**: Determine the exact strike price that minimizes total loss for all option holders and assess pin risk
- **get_strike_loss_breakdown**: Provide transparency by showing individual call and put losses at a specific strike
- **validate_market_data**: Ensure provided options data is logically consistent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Max Pain Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the max pain for these strikes: [100, 105, 110], call OI: [500, 200, 100], put OI: [100, 300, 600], and underlying price: 104."

**🤖 AI Agent:**
> The max pain strike is 105. The price distance is 1.0, and there is no pin risk.

---

**👤 You:**
> "Is there pin risk if the max pain strike is 150 and the current price is 150.5?"

**🤖 AI Agent:**
> Yes, there is pin risk because the price is within 1% of the max pain strike.

---

**👤 You:**
> "Show me the loss breakdown for strike 110 with strikes [100, 110, 120], call OI [100, 100, 100], and put OI [100, 100, 100]."

**🤖 AI Agent:**
> At strike 110, the call loss is 10000 and the put loss is 10000, resulting in a total loss of 20000.


## ❓ FAQ

**Q: What is the Max Pain point?**
The Max Pain point is the strike price where the total aggregate loss for all option holders is minimized, often used to estimate where market makers might drive the price.

**Q: How do I know if there is pin risk?**
The `calculate_max_pain` tool automatically flags pin risk if the underlying price is within 1% of the calculated max pain strike.

**Q: Can I see the individual losses for a strike?**
Yes, you can use the `get_strike_loss_breakdown` tool to view the specific call loss and put loss components for any candidate strike.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/max-pain-calculator](https://vinkius.com/ai-agent-connect/max-pain-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Max Pain Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `max-pain-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Max Pain Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "max-pain-calculator": {
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
