# EBITDA Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ebitda-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate EBITDA, margins, and EV/EBITDA multiples with industry benchmark comparisons.

## Description
The EBITDA Calculator MCP server provides essential tools for financial analysis. Use `calculate_earnings_metrics` to derive EBITDA and profitability margins from EBIT, depreciation, and amortization. With `calculate_enterprise_multiple`, you can determine valuation ratios using Enterprise Value. Finally, use `analyze_sector_variance` to compare your results against industry benchmarks like Technology or Energy to see if a company is undervalued or overvalued.


## Available Tools
- **analyze_sector_variance**: Compares the company's calculated multiple against predefined industry averages
- **calculate_earnings_metrics**: Calculates the fundamental EBITDA value and the resulting profitability margin
- **calculate_enterprise_multiple**: Calculates the current EV/EBITDA valuation multiple


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EBITDA Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate EBITDA and margin if EBIT is 100, depreciation is 20, amortization is 10, and revenue is 500."

**🤖 AI Agent:**
> The calculated EBITDA is 130.0 and the EBITDA margin is 26.0%.

---

**👤 You:**
> "What is the EV/EBITDA multiple if Enterprise Value is 1500 and EBITDA is 130?"

**🤖 AI Agent:**
> The EV/EBITDA multiple is approximately 11.54.

---

**👤 You:**
> "Compare a multiple of 11.54 against the Technology sector."

**🤖 AI Agent:**
> The variance is -23.07%, and the performance rating is Undervalued compared to the Technology benchmark of 15.0.


## ❓ FAQ

**Q: What metrics can I calculate with this server?**
You can calculate EBITDA, EBITDA margin, EV/EBITDA multiples, and compare them against sector benchmarks using tools like `calculate_earnings_metrics`.

**Q: How do I know if a company is undervalued?**
By using `analyze_sector_variance`, the server compares your calculated multiple to industry averages. A negative variance percentage indicates the company is cheaper than its sector benchmark.

**Q: Does this tool require an API key?**
No, this MCP server does not require any external API keys. It uses hardcoded sector benchmarks for comparison.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ebitda-calculator](https://vinkius.com/mcp/ebitda-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EBITDA Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ebitda-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EBITDA Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ebitda-calculator": {
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
