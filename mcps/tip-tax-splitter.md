# Tip & Tax Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tip-tax-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare pre-tax and post-tax bill splitting methods.

## Description
The Tip & Tax Splitter resolves the debate between proportional and additive bill splitting. Using `proportional_split`, you can calculate a split where tax and tip are distributed based on each person's share of the subtotal. Alternatively, use `additive_split` to see how much everyone pays when the entire group's tax and tip are applied to every individual. For a side-by-side comparison, use `compare_splits` to evaluate both methods at once.


## Available Tools (3)
- **additive_split**: Calculate a split where tax and even tip are distributed equally among all participants
- **compare_splits**: Compare proportional vs additive splitting methods
- **proportional_split**: Calculate a split where tax and tip are distributed proportionally to each person's subtotal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tip & Tax Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare the split for Alice ($20), Bob ($30) with 10% tax and 20% tip."

**🤖 AI Agent:**
> Proportional: Alice pays $26.00, Bob pays $39.00. Additive: Alice pays $53.00, Bob pays $66.00.

---

**👤 You:**
> "Calculate the proportional split for Charlie ($50) with 8% tax and 15% tip."

**🤖 AI Agent:**
> Charlie's total is $61.50 (Subtotal: $50, Tax: $4, Tip: $7.50).

---

**👤 You:**
> "Use additive_split for David ($10) and Eve ($40) with 5% tax and 10% tip."

**🤖 AI Agent:**
> David pays $60.00, Eve pays $100.00.


## ❓ FAQ

**Q: What is the difference between proportional and additive splitting?**
Proportional splitting (via `proportional_split`) distributes the group's total tax and tip based on how much each person spent. Additive splitting (via `additive_split`) applies the entire group's tax and tip amount to every single participant.

**Q: How can I see both methods at once?**
You can use the `compare_splits` tool to generate a structured comparison of both the proportional and additive methods side-by-side.

**Q: Do I need an API key to use this?**
No, you don't need any API keys. You can connect via Vinkius Edge using your personal Connection Token.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tip-tax-splitter](https://vinkius.com/mcp/tip-tax-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tip & Tax Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tip-tax-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tip & Tax Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tip-tax-splitter": {
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
