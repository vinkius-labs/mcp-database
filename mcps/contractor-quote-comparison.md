# Contractor Quote Comparison MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/contractor-quote-comparison)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Normalize contractor quotes into a comparison matrix and get negotiation intelligence.

## Description
This MCP server helps users compare multiple contractor bids by normalizing disparate line items into a single comparison matrix. It identifies scope mismatches, calculates coverage scores, and ranks options based on price or completeness. Use `analyze_quotes` to find gaps, `rank_options` to evaluate bids, `generate_negotiation_intelligence` for actionable checklists, and `validate_quote_integrity` to spot red flags like insufficient warranties.


## Available Tools (4)
- **generate_negotiation_intelligence**: Produces actionable documents for the user to use when talking to contractors
- **rank_options**: Evaluates and ranks the provided quotes based on price and coverage
- **validate_quote_integrity**: Checks for logical inconsistencies or "red flags" within individual quotes
- **analyze_quotes**: Normalizes multiple quotes into a standard comparison matrix and identifies scope gaps


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Contractor Quote Comparison** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare these three quotes for my kitchen remodel: [Quote A: $5000, includes cabinets], [Quote B: $4500, excludes cabinets], [Quote C: $6000, includes cabinets and sink]. My master scope is cabinets and sink."

**🤖 AI Agent:**
> The comparison shows Quote C has 100% coverage, Quote A has 50% coverage, and Quote B has 0% coverage for your required items.

---

**👤 You:**
> "Which contractor should I pick if I want the most complete work regardless of price?"

**🤖 AI Agent:**
> Based on the analysis, Contractor B is the best choice because they provide 100% coverage of your master scope.

---

**👤 You:**
> "Check this quote for any issues: {'price': 1200, 'warranty': 0, 'items': ['painting']}"

**🤖 AI Agent:**
> This quote contains a red flag: the warranty period is zero.


## ❓ FAQ

**Q: How do I compare multiple quotes?**
Use the `analyze_quotes` tool by providing the list of quotes and your master scope requirements.

**Q: Can I prioritize scope completeness over the lowest price?**
Yes, when using `rank_options`, set the `prioritizeCoverage` parameter to true.

**Q: What are red flags in a quote?**
You can use `validate_quote_integrity` to detect red flags such as warranties that are too short or exclusions that conflict with your required scope.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/contractor-quote-comparison](https://vinkius.com/en/ai-agent-connect/contractor-quote-comparison)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Contractor Quote Comparison** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `contractor-quote-comparison` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Contractor Quote Comparison** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "contractor-quote-comparison": {
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
