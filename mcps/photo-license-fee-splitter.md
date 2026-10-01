# Photo License Fee Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/photo-license-fee-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate photography license quotes, including gross client fees and net photographer payouts.

## Description
This MCP server provides tools to calculate photography licensing quotes. It determines multipliers for usage types, territories, and license terms to compute the final license fee. Use `calculate_license_quote` to generate both the gross fee for the client and the net fee for the photographer after agency commissions and taxes.


## Available Tools (4)
- **calculate_license_quote**: Performs the full calculation to generate a final quote for the client and the photographer
- **get_term_multiplier**: Determines the multiplier applied to the base fee based on the duration of the license
- **get_territory_multiplier**: If "world" is included, it returns the global multiplier.

Determines the multiplier applied to the base fee based on where the image will be used
- **get_usage_multiplier**: Determines the multiplier applied to the base fee based on the intended media usage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Photo License Fee Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a quote for a digital license with a $1000 base fee, used in the USA for 2 years, with a 20% agency commission and 10% tax."

**🤖 AI Agent:**
> The gross fee for the client is $2640.00 and the net fee for the photographer is $1600.00.

---

**👤 You:**
> "What is the multiplier for broadcast usage?"

**🤖 AI Agent:**
> The multiplier for broadcast usage is 5.0.

---

**👤 You:**
> "How much will the photographer receive for a $500 base fee, print usage, world territory, 1 year, 15% agency fee, and 5% tax?"

**🤖 AI Agent:**
> The gross fee is $1050.00 and the net fee for the photographer is $425.00.


## ❓ FAQ

**Q: How do I calculate the total cost for a client?**
You can use the `calculate_license_quote` tool by providing the base fee, usage type, territories, years, agency percentage, and tax rate.

**Q: What is the difference between gross and net fees?**
The gross fee is the total amount the client pays (including tax), while the net fee is the amount the photographer receives after the agency commission is deducted.

**Q: Can I find multipliers for specific media types?**
Yes, use the `get_usage_multiplier` tool to find the specific factor for digital, print, or broadcast usage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/photo-license-fee-splitter](https://vinkius.com/en/ai-agent-connect/photo-license-fee-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Photo License Fee Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `photo-license-fee-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Photo License Fee Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "photo-license-fee-splitter": {
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
