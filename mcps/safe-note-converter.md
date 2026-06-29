# Safe Note Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/safe-note-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate equity conversion, share issuance, and ownership dilution from SAFE conversions.

## Description
The Safe Note Converter is a specialized computational tool designed for founders and investors to simulate the complex equity conversion process of a SAFE (Simple Agreement for Future Equity). By using tools like `calculate_effective_conversion_price`, `calculate_shares_distributed`, and `calculate_ownership_stake`, you can accurately determine the impact of financing rounds on your capitalization table. The engine evaluates both valuation caps and discount rates to find the effective conversion price, calculates the exact number of shares issued based on the original investment, and determines the resulting ownership stake in the post-money scenario.


## Available Tools (3)
- **calculate_ownership_stake**: Calculates the investor's resulting ownership percentage
- **calculate_shares_distributed**: Calculates how many new common shares are issued to the SAFE holder
- **calculate_effective_conversion_price**: Determines the final price per


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Safe Note Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the effective conversion price if my valuation cap is $5,000,000, there are 10,000,000 shares outstanding, and the next round price is $0.60 with a 20% discount?"

**🤖 AI Agent:**
> The effective conversion price is $0.48. The discount-driven price ($0.48) was lower than the cap-driven price ($0.50).

---

**👤 You:**
> "If I invested $500,000 and the effective conversion price is $0.50, how many shares will I receive?"

**🤖 AI Agent:**
> You will receive 1,000,000 shares.

---

**👤 You:**
> "If I received 1,000,000 shares and the total post-money shares are 20,000,000, what is my ownership stake?"

**🤖 AI Agent:**
> Your ownership stake is 5.0%.


## ❓ FAQ

**Q: How does the effective conversion price calculation work?**
The `calculate_effective_conversion_price` tool compares two values: the price derived from the valuation cap and the price derived from the discount rate. It selects the lower of these two prices to ensure the investor receives the most favorable terms as defined in their SAFE agreement.

**Q: Can I calculate my post-conversion ownership percentage?**
Yes. By using the `calculate_ownership_stake` tool, you can provide the number of shares issued during conversion and the total post-money shares outstanding to find your exact ownership percentage.

**Q: What inputs are required for calculating shares distributed?**
To use `calculate_shares_distributed`, you need the original investment amount and the effective conversion price per share calculated in the previous step.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/safe-note-converter](https://vinkius.com/mcp/safe-note-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Safe Note Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `safe-note-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Safe Note Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "safe-note-converter": {
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
