# VIX Term Structure Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vix-term-structure-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze VIX futures term structure, roll yields, and market regimes.

## Description
This MCP server provides deterministic tools to analyze the VIX futures term structure. It identifies market regimes like Contango and Backwardation, calculates the theoretical roll yield between contracts, and determines the term structure slope using linear regression. Use `analyze_term_structure` to identify if the market is in a Complacent or Panic state, `calculate_roll_yield` to quantify returns when rolling positions, and `get_structure_slope` to find the price trend relative to time to expiration.


## Available Tools (3)
- **analyze_term_structure**: Determines the current market state and relationship between spot and futures
- **calculate_roll_yield**: Quantifies the return expected when rolling from the nearest contract to the next
- **get_structure_slope**: Calculates the trend of the term structure using linear regression


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VIX Term Structure Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the current VIX term structure with a spot of 15 and futures prices of [16, 17, 18] expiring in [10, 30, 50] days."

**🤖 AI Agent:**
> The market is in a Complacent regime with a positive slope, indicating a strong contango state.

---

**👤 You:**
> "What is the roll yield if M1 is 20, M2 is 18, and M1 expires in 15 days?"

**🤖 AI Agent:**
> -0.20

---

**👤 You:**
> "Calculate the slope for VIX futures priced at [25, 24, 23] with expirations at [5, 20, 40] days."

**🤖 AI Agent:**
> -0.1125


## ❓ FAQ

**Q: What is the difference between Contango and Backwardation?**
Contango occurs when futures prices are higher than the spot VIX, indicating low immediate fear. Backwardation occurs when futures prices are lower than the spot, indicating high immediate fear or panic.

**Q: How is the market regime determined?**
The regime is classified as Complacent if contango is greater than 5%, or Panic if backwardation is greater than 5%. Otherwise, it is considered Normal.

**Q: Can I calculate the roll yield for specific contracts?**
Yes, you can use `calculate_roll_yield` by providing the prices for the first and second month contracts and the days remaining until the first contract expires.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vix-term-structure-calculator](https://vinkius.com/mcp/vix-term-structure-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **VIX Term Structure Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vix-term-structure-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **VIX Term Structure Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vix-term-structure-calculator": {
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
