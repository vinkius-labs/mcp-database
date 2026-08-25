# Accelerator University Spinout Terms MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-university-spinout-terms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Generates equitable equity splits, royalty structures, and negotiation frameworks for university spinouts.

## Description
This MCP server provides decision-support tools for managing the complex transition from university research to commercial spinouts. It helps founders and Technology Transfer Offices (TTOs) reach fair agreements by calculating recommended equity distributions using `calculate_equity_split`, determining appropriate royalty percentages via `generate_royalty_structure`, and providing strategic roadmaps through `create_negotiation_framework`. The engine accounts for IP contribution weight, TTO policy constraints, and licensing types to ensure equitable outcomes for both researchers and institutions.


## Available Tools (3)
- **calculate_equity_split**: Recommends a specific equity distribution between the university and the founding team
- **create_negotiation_framework**: Provides a strategic roadmap for founders and TTO officers to reach an agreement
- **generate_royalty_structure**: Determines appropriate royalty percentages and milestone payment triggers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator University Spinout Terms** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Recommend an equity split where the IP weight is 0.7, the TTO requires 10% minimum, and the total range is between 10% and 30%."

**🤖 AI Agent:**
> The recommended university equity is 21% and the founder equity is 79%. This split accounts for the high IP contribution weight while respecting the TTO minimum requirement.

---

**👤 You:**
> "Generate a royalty structure for an exclusive license of core IP with a target revenue of 5,000,000."

**🤖 AI Agent:**
> The recommended royalty is 5% of net sales, with milestone payments triggered at $1M, $2.5M, and $5M in revenue, paid annually.

---

**👤 You:**
> "Create a negotiation framework for a founder-friendly stance using a 20/80 equity split and a 3% royalty structure."

**🤖 AI Agent:**
> To maintain a founder-friendly stance, focus on minimizing royalty percentages and maximizing equity retention. Key levers include negotiating lower milestone thresholds and emphasizing the need for founder liquidity to attract future investment.


## ❓ FAQ

**Q: How does the tool calculate the equity split?**
The `calculate_equity_split` tool uses the IP contribution weight and the minimum equity required by the TTO policy to recommend a distribution within the specified total equity range.

**Q: Can I generate a negotiation strategy?**
Yes, by using `create_negotiation_framework`, you can generate a strategic roadmap tailored to your specific stance, such as founder-friendly or university-conservative.

**Q: What factors influence the royalty structure?**
The `generate_royalty_structure` tool considers the licensing type, the qualitative importance of the IP, and the projected target revenue to determine royalty percentages and milestone payments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-university-spinout-terms](https://vinkius.com/ai-agent-connect/accelerator-university-spinout-terms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator University Spinout Terms** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-university-spinout-terms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator University Spinout Terms** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-university-spinout-terms": {
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
