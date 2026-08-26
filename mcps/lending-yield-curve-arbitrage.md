# Lending Yield Curve Arbitrage MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/lending-yield-curve-arbitrage)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Identify and evaluate profitable yield arbitrage loops between stablecoin lending protocols.

## Description
This MCP server provides a deterministic toolset for identifying and evaluating yield arbitrage opportunities between decentralized lending protocols. By analyzing the yield spread between different stablecoin pools, users can identify profitable loops where they borrow from one protocol and supply to another. The server includes tools like `find_arbitrage_opportunities` to scan for valid spreads, `evaluate_loop_economics` to calculate net yield and liquidation risks, and `get_protocol_safety_score` to assess protocol maturity and liquidity. It enforces strict safety rules, such as minimum TVL requirements and age thresholds, to mitigate smart contract risk.


## Available Tools (3)
- **find_arbitrage_opportunities**: Identifies valid arbitrage loops between different lending protocols for stablecoin pairs
- **evaluate_loop_economics**: Calculates the net profitability and risk metrics for a specific identified arbitrage opportunity
- **get_protocol_safety_score**: Provides a qualitative risk assessment of a protocol based on its operational history and liquidity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lending Yield Curve Arbitrage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find arbitrage opportunities between Aave and Compound for USDC."

**🤖 AI Agent:**
> The identified opportunity is to borrow USDC from Compound at 3.5% and supply it to Aave at 5.2%, resulting in a yield spread of 1.7%. However, this does not meet the minimum 2% spread requirement.

---

**👤 You:**
> "Calculate the economics for a 100,000 USDC arbitrage loop with a 1% risk buffer."

**🤖 AI Agent:**
> The net yield for this loop is 3.45% after accounting for the liquidation risk buffer and gas costs. The loop LTV is 65%, and the liquidation price is set at a 20% deviation from current levels.

---

**👤 You:**
> "Is the Morpho protocol considered safe for this strategy?"

**🤖 AI Agent:**
> Yes, Morpho is considered a trusted protocol as it meets the minimum age and TVL requirements for this strategy.


## ❓ FAQ

**Q: How do I find valid arbitrage opportunities?**
Use the `find_arbitrage_opportunities` tool with your lending and borrowing rate data. It will return valid loops where the yield spread exceeds the required safety thresholds.

**Q: How is the net yield calculated?**
The net yield is determined by the `evaluate_loop_economics` tool, which subtracts the liquidation risk buffer and the gas costs amortized over the expected duration from the gross yield spread.

**Q: What safety checks are performed on protocols?**
The server uses `get_protocol_safety_score` to ensure protocols meet minimum TVL and age requirements, reducing exposure to smart contract risk.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/lending-yield-curve-arbitrage](https://vinkius.com/ai-agent-connect/lending-yield-curve-arbitrage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lending Yield Curve Arbitrage** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lending-yield-curve-arbitrage` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lending Yield Curve Arbitrage** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lending-yield-curve-arbitrage": {
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
