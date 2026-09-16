# Venture Redemption Rights MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-redemption-rights)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates the financial economics, solvency risks, and probabilities of venture capital redemption rights.

## Description
This MCP server provides specialized tools for modeling the economic impact of venture capital redemption rights. It allows investors and analysts to calculate the `get_redemption_value` based on company cash, measure `calculate_downside_protection` against investment loss, estimate the `evaluate_trigger_probability` based on time and growth, and verify legal compliance using `check_legal_solvency` under USA and European standards.


## Available Tools (4)
- **evaluate_trigger_probability**: Estimates the likelihood that a redemption event will occur based on the time remaining and the company's operational state
- **get_redemption_value**: Determines the total economic value an investor stands to receive if the redemption is successfully triggered
- **calculate_downside_protection**: Measures the degree of protection the redemption right provides against total loss of investment
- **check_legal_solvency**: Evaluates whether a redemption can be legally executed under USA and European solvency standards


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Redemption Rights** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the redemption value for a $5,000,000 redemption price with $3,000,000 in company cash."

**🤖 AI Agent:**
> The theoretical redemption value is $5,000,000, but the effective payout is $3,000,000 due to the current cash position, leaving a solvency gap of $2,000,000.

---

**👤 You:**
> "What is the downside protection for a $1,000,000 redemption with a 0.5 trigger probability and $800,000 cash?"

**🤖 AI Agent:**
> The expected recovery value is $500,000, with a risk exposure of $500,000 based on the provided probability and cash constraints.

---

**👤 You:**
> "Check if a $2,000,000 redemption is legal if the company has $2,500,000 cash and $1,000,000 in total liabilities."

**🤖 AI Agent:**
> The redemption is legally viable. After paying the $2,000,000, the company maintains a solvency margin of $500,000 above its liabilities.


## ❓ FAQ

**Q: How does this tool handle solvency constraints?**
The `check_legal_solvency` tool evaluates if a redemption request would violate legal requirements by comparing the company's cash position against its total liabilities.

**Q: Can I calculate the actual payout if the company has low cash?**
Yes, using `get_redemption_value`, you can determine the effective payout, which is the lesser of the redemption price or the available company cash.

**Q: What factors influence the trigger probability?**
The `evaluate_trigger_probability` tool uses the redemption period, years elapsed, and the company's growth trajectory to estimate the likelihood of a redemption event.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-redemption-rights](https://vinkius.com/en/ai-agent-connect/venture-redemption-rights)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Redemption Rights** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-redemption-rights` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Redemption Rights** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-redemption-rights": {
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
