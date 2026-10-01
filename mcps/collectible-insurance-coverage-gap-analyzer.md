# Collectible Insurance Coverage Gap Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/collectible-insurance-coverage-gap-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate insurance coverage gaps and inflation-adjusted valuations for collectibles.

## Description
This MCP server provides specialized tools to bridge the gap between collectible market values and insurance policy protections. Use `calculate_item_coverage` to find the specific financial protection for a single item, or `analyze_category_exposure` to evaluate risk across an entire category. It also includes `calculate_inflation_adjusted_valuation` to update historical prices and `compare_policy_vs_market` for high-level portfolio assessments.


## Available Tools (4)
- **calculate_inflation_adjusted_valuation**: Updates a historical valuation to reflect current market conditions
- **calculate_item_coverage**: Determines the specific financial protection for a single collectible item
- **compare_policy_vs_market**: A high-level comparison between total market holdings and total insurance availability
- **analyze_category_exposure**: Evaluates the total risk for a group of items within a single insurance category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Collectible Insurance Coverage Gap Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My rare coin is worth $5,000, but my category limit is $4,000 and my deductible is $200. How much is covered?"

**🤖 AI Agent:**
> The covered value is $3,800, and the uncovered gap is $1,200.

---

**👤 You:**
> "I bought a comic book for $100 years ago. With a 5% inflation rate, what is it worth now?"

**🤖 AI Agent:**
> The adjusted value is $105.00.

---

**👤 You:**
> "Compare my total market holdings of $50,000 against policy limits of $45,000 and total deductibles of $1,000."

**🤖 AI Agent:**
> The total coverage gap is $6,000, the total potential payout is $44,000, and the coverage ratio is 0.88.


## ❓ FAQ

**Q: How does the tool handle scheduled items?**
When using `calculate_item_coverage`, providing a `scheduledLimit` ensures the tool uses the specific coverage amount assigned to that high-value item instead of the general category limit.

**Q: Can I adjust for inflation?**
Yes, the `calculate_inflation_adjusted_valuation` tool allows you to update historical valuations to current market conditions using a specified inflation rate.

**Q: What is the uncovered gap?**
The uncovered gap is the difference between the current market valuation of your collectible and the actual amount covered by your insurance policy after the deductible.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/collectible-insurance-coverage-gap-analyzer](https://vinkius.com/en/ai-agent-connect/collectible-insurance-coverage-gap-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Collectible Insurance Coverage Gap Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `collectible-insurance-coverage-gap-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Collectible Insurance Coverage Gap Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "collectible-insurance-coverage-gap-analyzer": {
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
