# CD Return Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cd-return-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate potential returns on Certificates of Deposit (CD) and compare them against market benchmarks like HYSA and Money Market funds.

## Description
The CD Return Calculator is a specialized financial tool designed to help you project the growth of your investments in Certificates of Deposit. By providing the principal amount, APY, and term duration, you can use tools like `calculate_cd_yield` to see exactly how much interest you will earn and what your final balance will be. The server also provides context by using `fetch_market_benchmarks` to compare your CD's performance against current High-Yield Savings Account (HYSA) and Money Market rates. Finally, the `generate_investment_comparison` tool produces a clear assessment of whether your CD is outperforming liquid market alternatives.


## Available Tools
- **calculate_cd_yield**: Calculates the growth of an investment based on CD terms and compounding interest
- **fetch_market_benchmarks**: Retrieves the current hardcoded benchmark rates for liquid alternatives based on a given interest rate level
- **generate_investment_comparison**: Produces a high-level comparison between the CD investment and market alternatives


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CD Return Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the return for a $5,000 CD with 4.5% APY for 12 months, compounding monthly."

**🤖 AI Agent:**
> For a $5,000 deposit at 4.5% APY over 12 months with monthly compounding, your total interest earned will be $229.36, resulting in a final balance of $5,229.36.

---

**👤 You:**
> "Is a 4% CD better than current market benchmarks?"

**🤖 AI Agent:**
> Based on current benchmarks, a 4% CD is performing similarly to the available HYSA and Money Market rates in this tier.

---

**👤 You:**
> "Compare a $10,000 CD at 5% APY for 24 months against HYSA rates."

**🤖 AI Agent:**
> A $10,000 CD at 5% APY for 24 months will yield a final balance of $11,049.41. This outperforms the current HYSA benchmark rate.


## ❓ FAQ

**Q: How does the calculator determine my final balance?**
The `calculate_cd_yield` tool applies your specified compounding frequency (daily, monthly, quarterly, or annually) to the principal amount over the chosen term to calculate total interest and the final balance.

**Q: Can I compare my CD rate to other savings options?**
Yes. By using `fetch_market_benchmarks`, the tool retrieves current benchmark rates for HYSA and Money Market funds, allowing you to see how your CD compares to liquid alternatives.

**Q: What does the advantage score represent?**
The advantage score, generated via `generate_investment_comparison`, represents the numeric margin between your CD's APY and the relevant market benchmark rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cd-return-calculator](https://vinkius.com/mcp/cd-return-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CD Return Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cd-return-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CD Return Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cd-return-calculator": {
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
