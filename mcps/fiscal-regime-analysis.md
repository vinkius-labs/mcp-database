# Fiscal Regime Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fiscal-regime-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze economic outcomes for oil and gas projects using Concessionary and PSC models.

## Description
This MCP server provides specialized tools to evaluate the fiscal impact of hydrocarbon extraction. It allows users to calculate government and contractor takes, effective tax rates, and net profits under different legal frameworks. Use `analyze_concession_economics` for concession-based projects, `analyze_psc_economics` for Production Sharing Contracts, and `compare_regimes` to determine which model yields a higher contractor take for a specific scenario. It also includes `get_fiscal_summary` for high-level economic splits.

### Available Tools

`analyze_concession_tool`, `analyze_psc_tool`, `compare_regimes_tool`, `get_fiscal_summary_tool`


## Available Tools (4)
- **analyze_psc_tool**: Evaluates the fiscal outcome for a project operating under a Production Sharing Contract (PSC)
- **compare_regimes_tool**: Provides a direct comparison between a Concessionary model and a PSC model
- **get_fiscal_summary_tool**: Generates a high-level summary of the economic split for a given project scenario
- **analyze_concession_tool**: Evaluates the fiscal outcome for a project operating under a Concessionary regime


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fiscal Regime Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the economics for a concession project with $1,000,000 revenue, 10% royalty, 30% tax, and $500,000 operating costs."

**🤖 AI Agent:**
> The government take is $190,000, the contractor take is $310,000, and the effective tax rate is 19%.

---

**👤 You:**
> "Compare a concession model (1000 revenue, 0.1 royalty, 0.3 tax, 500 costs) with a PSC model (1000 revenue, 0.7 cost limit, 0.5 profit split, 500 costs, 0.3 tax)."

**🤖 AI Agent:**
> The PSC model is the winner for the contractor.

---

**👤 You:**
> "What is the economic split if the government takes $400 and the contractor takes $600?"

**🤖 AI Agent:**
> The total value is $1,000, with a 40% government share and a 60% contractor share.


## ❓ FAQ

**Q: What is the difference between the two models?**
The Concessionary model involves the contractor paying royalties and taxes, while the Production Sharing Contract (PSC) involves splitting 'profit oil' after cost recovery. Tools available: `analyze_concession_tool`, `analyze_psc_tool`, `compare_regimes_tool`.

**Q: How can I compare two different fiscal models?**
You can use the `compare_regimes` tool by providing the parameters for both the concessionary and PSC models.

**Q: Can I get a summary of the economic split?**
Yes, the `get_fiscal_summary` tool provides the total value and the percentage split between the government and the contractor.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fiscal-regime-analysis](https://vinkius.com/en/ai-agent-connect/fiscal-regime-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fiscal Regime Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fiscal-regime-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fiscal Regime Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fiscal-regime-analysis": {
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
