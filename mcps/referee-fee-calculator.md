# Referee Fee Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/referee-fee-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate referee compensation based on match counts and tiered fee structures.

## Description
This MCP server provides tools to manage and calculate referee compensation. It allows users to retrieve standard regional fees using `get_base_fee`, calculate simple totals with `calculate_match_total`, determine compensation tiers via `get_tiered_fee_rate`, and compute final payouts including volume bonuses with `calculate_volume_bonus_total`.


## Available Tools (4)
- **calculate_match_total**: Calculate the total fee for a set number of matches
- **calculate_volume_bonus_total**: Calculate total payment including volume-based tier increases
- **get_base_fee**: Get the standard fee and currency for a specific region
- **get_tiered_fee_rate**: Get the applicable fee rate based on match volume


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Referee Fee Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the standard fee for a match in the USA?"

**🤖 AI Agent:**
> The standard fee for a match in the USA is 50 USD.

---

**👤 You:**
> "How much is the total pay for 10 matches at 40 per match?"

**🤖 AI Agent:**
> The total pay for 10 matches at 40 per match is 400.

---

**👤 You:**
> "What tier is an official in after 50 matches?"

**🤖 AI Agent:**
> An official with 50 matches has reached the Professional Tier.


## ❓ FAQ

**Q: How do I find the standard fee for a specific region?**
You can use the `get_base_fee` tool and provide the region name, such as 'USA' or 'Europe'.

**Q: Can I calculate total pay including volume bonuses?**
Yes, use the `calculate_volume_bonus_total` tool to get the final payout considering tiered increases.

**Q: What happens if I provide an invalid region?**
The `get_base_fee` tool will return an error if the requested region is not supported in the regional standards catalog.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/referee-fee-calculator](https://vinkius.com/en/ai-agent-connect/referee-fee-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Referee Fee Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `referee-fee-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Referee Fee Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "referee-fee-calculator": {
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
