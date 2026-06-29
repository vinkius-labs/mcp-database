# Dilution Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dilution-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Simulate equity dilution, cap table evolution, and anti-dilution adjustments during investment rounds.

## Description
The Dilution Calculator is a specialized simulation engine designed for founders and investors to model the impact of new funding rounds on existing equity. Using tools like `calculate_round_dilution` and `simulate_option_pool_expansion`, you can predict how much current shareholders will be diluted by new capital, how an expanded ESOP affects ownership, and evaluate the consequences of down rounds using `calculate_anti_dilution_impact`. It provides a clear view of your cap table evolution through `get_cap_table_snapshot`.


## Available Tools (4)
- **calculate_round_dilution**: Simulates a new investment round
- **calculate_anti_dilution_impact**: Evaluates Broad-Based Weighted Average anti-dilution impact
- **get_cap_table_snapshot**: Provides a clear view of the current ownership structure
- **simulate_option_pool_expansion**: Calculates effective dilution from ESOP resizing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dilution Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my current ownership structure?"

**🤖 AI Agent:**
> The current cap table shows: Founder A (40%), Founder B (30%), Angel Investor (20%), and ESOP (10%). Total shares outstanding: 1,000,000.

---

**👤 You:**
> "If we raise $2M at a $8M pre-money valuation, what happens to our ownership?"

**🤖 AI Agent:**
> The post-money valuation will be $10M. The new investors will hold 20% of the company, and existing shareholders will experience a dilution factor of 0.8.

---

**👤 You:**
> "Calculate the impact of an anti-dilution adjustment if our previous price was $1.50 and the new price is $1.20."

**🤖 AI Agent:**
> The Broad-Based Weighted Average calculation results in a new conversion price of $1.42, with an adjustment ratio of 0.95.


## ❓ FAQ

**Q: How does the calculator handle option pool expansion?**
The `simulate_option_pool_expansion` tool calculates the additional shares required to reach a target post-money ESOP size, specifically showing the impact on founder ownership.

**Q: Can I simulate a down round?**
Yes. By using `calculate_anti_dilution_impact`, you can evaluate how a Broad-Based Weighted Average anti-dilution clause will adjust conversion prices when the new share price is lower than previous rounds.

**Q: What information do I need for a round simulation?**
To use `calculate_round_dilution`, you need the new investment amount and the pre-money valuation. You can also optionally include a target option pool expansion percentage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dilution-calculator](https://vinkius.com/mcp/dilution-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dilution Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dilution-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dilution Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dilution-calculator": {
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
