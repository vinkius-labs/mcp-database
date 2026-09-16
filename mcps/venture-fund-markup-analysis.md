# Venture Fund Markup Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-fund-markup-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze venture capital fund performance through markup velocity and valuation quality.

## Description
This MCP server provides deep insights into venture capital fund performance. It allows AI agents to evaluate how quickly portfolio companies are growing using `analyze_markup_velocity`, assess the reliability of unrealized gains with `evaluate_valuation_quality`, and identify the gap between paper wealth and cash exits via `calculate_return_divergence`. Additionally, it can detect artificial valuation shifts using `track_methodology_impact`.


## Available Tools (4)
- **analyze_markup_velocity**: Determines the rate of valuation growth for a specific company
- **track_methodology_impact**: g. multiples to DCF) artificially changed the valuation.

Analyzes how changes in valuation logic affect reported fund performance
- **calculate_return_divergence**: Compares theoretical paper gains against actual cash realized
- **evaluate_valuation_quality**: Assesses the reliability of the current unrealized gains


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Fund Markup Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How fast is company ABC's valuation growing over the last 4 quarters?"

**🤖 AI Agent:**
> Company ABC has shown a steady upward trend with a velocity rate of 15% per quarter over the last four quarters.

---

**👤 You:**
> "Is the current valuation for company XYZ reliable?"

**🤖 AI Agent:**
> The valuation for company XYZ is considered high quality as it was supported by a funding round in the last two quarters.

---

**👤 You:**
> "What is the divergence between paper and realized returns for Fund Alpha?"

**🤖 AI Agent:**
> Fund Alpha has a paper return of 45% and a realized return of 12%, resulting in a divergence gap of 33%.


## ❓ FAQ

**Q: How do I check if a company's valuation is growing quickly?**
You can use the `analyze_markup_velocity` tool to determine the rate of valuation growth for a specific company over a set number of quarters.

**Q: What is the difference between paper returns and realized returns?**
Paper returns are the theoretical gains shown on the fund's books from markups, while realized returns are the actual cash distributed from exits. Use `calculate_return_divergence` to find the gap between them.

**Q: Can I see if a valuation change was caused by a change in accounting logic?**
Yes, the `track_methodology_impact` tool analyzes how shifts in valuation methodology affect reported performance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-fund-markup-analysis](https://vinkius.com/en/ai-agent-connect/venture-fund-markup-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Fund Markup Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-fund-markup-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Fund Markup Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-fund-markup-analysis": {
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
