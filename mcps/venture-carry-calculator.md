# Venture Carry Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-carry-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate carried interest distributions, waterfall tiers, and clawback liabilities.

## Description
This MCP server provides precise tools for venture fund distribution modeling. It handles the full waterfall sequence, including return of capital, preferred returns, and GP catch-up provisions. Use `get_full_waterfall_distribution` to model the complete distribution flow, `check_hurdle_status` to verify if preferred returns are met, and `calculate_clawback_liability` to ensure GP distributions remain within agreed limits. It is designed for fund managers and LPs to model complex carried interest scenarios accurately.


## Available Tools (4)
- **check_hurdle_status**: Checks if the fund has met the minimum return required for the GP to begin receiving carry
- **calculate_clawback_liability**: Determines if the GP owes money back to the LPs based on realized performance
- **get_full_waterfall_distribution**: Provides a complete breakdown of the entire distribution process from gross proceeds to final split
- **validate_gp_commitment_alignment**: Validates if the GP's financial commitment is sufficient according to specific fund rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Carry Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the waterfall distribution for $100M gross proceeds, $60M LP capital, 10% GP commitment, 20% carry, and an 8% hurdle rate with catch-up."

**🤖 AI Agent:**
> The distribution includes $60M return of capital, $4.8M preferred return, and the subsequent GP catch-up and pro-rata split based on the $40M total profit.

---

**👤 You:**
> "Has the hurdle been met for a fund with $50M proceeds, $45M LP capital, and a 5% hurdle rate?"

**🤖 AI Agent:**
> No, the hurdle has not been met. The required preferred return is $2.25M, but only $5M in profit is available after capital return.

---

**👤 You:**
> "Check if the GP owes a clawback if they have received $5M in carry so far, but current proceeds and LP capital result in only $4M of entitled carry."

**🤖 AI Agent:**
> Yes, a clawback is triggered. The GP must return $1,000,000 to the LPs.


## ❓ FAQ

**Q: How do I calculate the full distribution breakdown?**
You can use the `get_full_waterfall_distribution` tool by providing gross proceeds, LP capital, GP commitment, carry percentage, and the hurdle rate.

**Q: Can this tool detect if a GP owes money back to LPs?**
Yes, the `calculate_clawback_liability` tool determines if the GP's total carry distributed to date exceeds their entitlement based on current proceeds.

**Q: How do I check if the preferred return has been satisfied?**
Use the `check_hurdle_status` tool to see if the fund has met the minimum return required for the GP to begin receiving carry.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-carry-calculator](https://vinkius.com/en/ai-agent-connect/venture-carry-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Carry Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-carry-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Carry Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-carry-calculator": {
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
