# Venture Co-Investment Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-co-investment-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze co-investment economics, LP profitability, and allocation strategies.

## Description
This MCP server provides specialized tools for Limited Partners (LPs) to evaluate co-investment opportunities. It calculates the net return advantage using `get_return_advantage`, models total LP profitability with `calculate_lp_economics`, and provides strategic guidance via `evaluate_allocation_strategy`. It helps LPs understand the impact of fee waivers, carry sharing, and minimum commitment requirements to make informed capital allocation decisions.


## Available Tools (3)
- **evaluate_allocation_strategy**: Provide guidance on whether to commit capital based on rights and requirements
- **calculate_lp_economics**: Model the total profit and loss for the Limited Partner
- **get_return_advantage**: Determine how much more efficient the co-investment is compared to the primary fund


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Co-Investment Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the LP economics for a $5M co-investment with a $50M exit value, 20% carry sharing, and no fee waiver."

**🤖 AI Agent:**
> The total profit is $35,000,000 with an effective multiple of 8.0x and a net yield of 700%.

---

**👤 You:**
> "Is a $2M co-investment advantageous if the primary fund returns 15%, the co-investment returns 18%, and fees are waived?"

**🤖 AI Agent:**
> Yes, the co-investment provides a significant net return advantage due to the fee waiver.

---

**👤 You:**
> "I want to invest $1M, but the minimum commitment is $2M and I don't have specific access rights. What should I do?"

**🤖 AI Agent:**
> The recommendation is to Decline, as the proposed amount is below the minimum commitment and no access rights are present.


## ❓ FAQ

**Q: How does this tool help with LP economics?**
You can use `calculate_lp_economics` to model total profit, effective multiples, and net yields based on projected exit values and carry sharing percentages.

**Q: Can I evaluate if a co-investment is better than the main fund?**
Yes, the `get_return_advantage` tool compares the efficiency of the co-investment against the primary fund, accounting for fee waivers.

**Q: How are allocation recommendations made?**
The `evaluate_allocation_strategy` tool provides recommendations by analyzing your commitment amount against minimum requirements and access rights.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-co-investment-analyzer](https://vinkius.com/en/ai-agent-connect/venture-co-investment-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Co-Investment Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-co-investment-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Co-Investment Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-co-investment-analyzer": {
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
