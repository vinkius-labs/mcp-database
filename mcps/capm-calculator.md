# CAPM Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/capm-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate expected asset returns using the Capital Asset Pricing Model (CAPM) and evaluate investment attractiveness.

## Description
The CAPM Calculator is a specialized tool for investors to determine the theoretically appropriate required rate of return of an asset. By considering systematic risk relative to the market, it uses the `calculate_expected_return` tool to compute returns based on Beta, Risk-Free Rate, and regional Equity Risk Premium (ERP). Additionally, you can use `analyze_asset_performance` to measure Alpha and determine if an investment is 'Attractive' or 'Unobstructive'. The system includes `get_regional_erp` to fetch standardized risk compensation values for the USA, Europe, and Brazil markets.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **CAPM Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected return for an asset with a beta of 1.2, a risk-free rate of 3%, in the USA market?"

**🤖 AI Agent:**
> The expected return for the asset is 9.9%.

---

**👤 You:**
> "If an asset in Brazil has a beta of 0.8 and the risk-free rate is 5%, what is its expected return?"

**🤖 AI Agent:**
> The expected return for the asset in Brazil is 10.6%.

---

**👤 You:**
> "An asset has an actual return of 8% and an expected return of 7.5%. Is it a good investment?"

**🤖 AI Agent:**
> Yes, the asset is considered Attractive because it has a positive Alpha of 0.5%.


## ❓ FAQ

**Q: What is the purpose of this tool?**
This tool calculates the expected return of an asset using the Capital Assetting Pricing Model (CAPM) and evaluates its performance by calculating Alpha. Tools available: `your_tool_name`.

**Q: How is the Equity Risk Premium (ERP) determined?**
The ERP is hardcoded for specific regions: 4.5% for the USA, 5% for Europe, and 7% for Brazil.

**Q: What does an 'Attractive' rating mean?**
An asset is rated 'Attractive' if its Alpha (the difference between actual and expected return) is zero or greater.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/capm-calculator](https://vinkius.com/mcp/capm-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CAPM Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `capm-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CAPM Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "capm-calculator": {
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
