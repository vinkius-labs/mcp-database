# Tax Regime Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tax-regime-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Simulate and compare Brazilian tax regimes to find the most cost-effective structure for your business.

## Description
The Tax Regime Comparator is a specialized financial simulation engine designed to help businesses navigate the complexities of Brazilian taxation. By analyzing projected annual revenue, profit margins, and business activity types, this MCP server provides precise comparisons between Simples Nacional, Lucro Presumido, and Lucro Real. Use `compare_tax_regimes` to identify the optimal regime and potential savings, or use `get_regime_breakdown` for a granular view of specific tax components like IRPJ and CSLL.


## Available Tools (2)
- **compare_tax_regimes**: Compares different Brazilian tax regimes to find the most efficient one
- **get_regime_breakdown**: Provides a detailed breakdown of tax components for a specific regime


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tax Regime Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare tax regimes for a service company with 500,000 BRL annual revenue and a 30% profit margin."

**🤖 AI Agent:**
> Based on your inputs, the best regime is Simples Nacional, with an estimated total tax of 45,000 BRL and a potential savings of 12,000 BRL compared to Lucro Presumido.

---

**👤 You:**
> "What is the tax breakdown for Lucro Real in a manufacturing business with 2,000,000 BRL revenue?"

**🤖 AI Agent:**
> For the Lucro Real regime, your total tax is 180,000 BRL. This includes Federal Tax components of 120,000 BRL and Municipal Tax components of 60,000 BRL.

---

**👤 You:**
> "If my profit margin increases to 40%, will the optimal tax regime change?"

**🤖 AI Agent:**
> No, at a 40% profit margin with your current revenue, Simples Nacional remains the most advantageous option.


## ❓ FAQ

**Q: How does the comparison work?**
The tool uses your projected revenue and profit margin to calculate the total tax burden under three different legal frameworks: Simples Nacional, Lucro Presumido, and Lucro Real.

**Q: What business activities are supported?**
The comparator currently supports TRADE, SERVICES, and MANUFACTURING activity types.

**Q: Can I see a detailed breakdown of taxes?**
Yes, you can use the `get_regime_breakdown` tool to see individual tax components like Federal and Municipal taxes for a specific regime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tax-regime-comparator](https://vinkius.com/mcp/tax-regime-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tax Regime Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tax-regime-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tax Regime Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tax-regime-comparator": {
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
