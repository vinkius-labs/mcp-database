# Venture ROFR Economics Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-rofr-economics-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Quantify the financial impact and liquidity trade-offs of Right of First Refusal (ROFR) provisions.

## Description
This MCP server provides a specialized economic modeling engine for venture capital professionals. It quantifies the financial implications of Right of First Refusal (ROFR) provisions by analyzing transfer constraints and liquidity trade-offs. Use `get_rofr_valuation` to determine the monetary value of an option, `analyze_transfer_restriction` to measure exit friction, `calculate_co_sale_impact` to evaluate co-sale rights, and `evaluate_liquidity_tradeoff` to synthesize a complete liquidity profile.


## Available Tools (4)
- **calculate_co_sale_impact**: Evaluates how co-sale rights affect the economic distribution of a transfer
- **evaluate_liquidity_tradeoff**: Synthesizes the economic value and the transfer friction to provide a single liquidity profile
- **get_rofr_valuation**: Determines the monetary value of the ROFR option based on a pending sale
- **analyze_transfer_restriction**: Quantifies the impact of the ROFR on the seller's ability to exit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture ROFR Economics Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the value of a ROFR option if the offer is $1,000,000 for 50,000 shares and the holder has a 20% right?"

**🤖 AI Agent:**
> The ROFR value is $200,000.

---

**👤 You:**
> "Calculate the liquidity risk for a transfer with a 60-day notice period and a market activity index of 0.8."

**🤖 AI Agent:**
> The liquidity risk is High.

---

**👤 You:**
> "If a seller offers 10,000 shares at $50 each and co-sale holders are entitled to 2,000 shares, what is the remaining value for the seller?"

**🤖 AI Agent:**
> The remaining seller value is $400,000.


## ❓ FAQ

**Q: How does this tool help with ROFR analysis?**
It provides precise mathematical models to calculate the value of ROFR options and the friction caused by transfer restrictions.

**Q: Can I model the impact of co-sale rights?**
Yes, the `calculate_co_sale_impact` tool evaluates how co-sale rights affect the economic distribution between primary sellers and co-sale holders.

**Q: What is the difference between a permitted transfer and a restricted one?**
Permitted transfers are exceptions that do not trigger ROFR, resulting in zero friction. Restricted transfers trigger the ROFR process, which can introduce delays and economic friction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-rofr-economics-engine](https://vinkius.com/en/ai-agent-connect/venture-rofr-economics-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture ROFR Economics Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-rofr-economics-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture ROFR Economics Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-rofr-economics-engine": {
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
