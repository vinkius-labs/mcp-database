# PE Ratio Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pe-ratio-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze stock valuation using P/E, PEG, and sector-specific benchmarks.

## Description
The PE Ratio Analyzer is a specialized tool for fundamental equity valuation. It allows users to calculate critical metrics such as Trailing P/E, Forward P/E, PEG Ratio, P/S Ratio, and EV/EBITDA. By using tools like `calculate_earnings_ratios` and `evaluate_valuation_status`, investors can compare current market multiples against sector-specific benchmarks (e.g., Tech or General) to identify if a stock is overvalued, undervalued, or fairly priced.


## Available Tools (4)
- **calculate_earnings_ratios**: Determine current and projected price-to-earnings multiples
- **calculate_growth_ratio**: Assess valuation relative to expected company expansion
- **calculate_revenue_enterprise_ratios**: Compute valuation multiples based on top-line revenue and enterprise earnings
- **evaluate_valuation_status**: Classify a stock as overvalued, undervalued, or fairly priced


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PE Ratio Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is Apple currently overvalued? The price is $190, trailing EPS is $6.00, and it's in the tech sector."

**🤖 AI Agent:**
> Apple's trailing P/E ratio is 31.67x. Based on the tech sector benchmark of 25-30x, it is classified as Overvalued.

---

**👤 You:**
> "Calculate the PEG ratio for a company with a P/E of 20 and an expected growth rate of 15%."

**🤖 AI Agent:**
> The calculated PEG ratio is 1.33.

---

**👤 You:**
> "What is the P/S ratio if the price is $50 and revenue per share is $5?"

**🤖 AI Agent:**
> The P/S ratio is 10.0.


## ❓ FAQ

**Q: How do I calculate the PEG ratio?**
You can use the `calculate_growth_ratio` tool. Provide the current P/E ratio and the expected annual earnings growth rate as a decimal.

**Q: What sectors are supported for benchmarking?**
The tool currently supports 'general' (S&P 500 average) and 'tech' sectors to determine if a stock is overvalued or undervalued.

**Q: Can I calculate the P/S ratio?**
Yes, use the `calculate_revenue_enterprise_ratios` tool by providing the share price, revenue per share, enterprise value, and EBITDA.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pe-ratio-analyzer](https://vinkius.com/mcp/pe-ratio-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PE Ratio Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pe-ratio-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PE Ratio Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pe-ratio-analyzer": {
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
