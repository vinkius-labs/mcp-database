# ICMS Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/icms-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Brazilian ICMS taxes, including tax substitution (ST), tax differentials (DIFAL), and tax-inclusive base calculations.

## Description
This MCP server provides specialized tools for calculating complex Brazilian ICMS taxes. It handles the 'inside' calculation method to find grossed-up product values, calculates Tax Substitution (ICMS-ST) using MVA (Added Value Margin), determines the tax differential (DIFAL) for B2C interstate transactions, and retrieves correct interstate rates based on regional movements. Use `calculate_tax_base` for tax-inclusive bases, `calculate_icms_substitution` for ST calculations, `calculate_tax_differential` for DIFAL, and `get_interstate_rate` to identify applicable rates between Brazilian regions.


## Available Tools (4)
- **calculate_tax_differential**: Calculates the DIFAL amount for B2C interstate operations
- **calculate_icms_substitution**: Calculates the amount of ICMS-ST (Tax Substitution) to be collected
- **calculate_tax_base**: Calculates the grossed-up product value using the "inside" calculation method
- **get_interstate_rate**: Retrieves the correct interstate tax rate based on origin and destination regions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ICMS Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the tax base for a product worth 100.00 with an 18% tax rate."

**🤖 AI Agent:**
> The `calculate_tax_base` tool would return a tax base of approximately 121.95 and a tax amount of 21.95.

---

**👤 You:**
> "What is the interstate rate for a shipment from Southeast to North region?"

**🤖 AI Agent:**
> Using `get_interstate_rate` with origin 'Southeast' and destination 'North', the tool returns a rate of 7%.

---

**👤 You:**
> "Calculate DIFAL for a product worth 500.00, with an interstate rate of 12% and destination internal rate of 18%."

**🤖 AI Agent:**
> The `calculate_tax_differential` tool calculates a DIFAL amount of 30.00.


## ❓ FAQ

**Q: How do I calculate the grossed-up product value?**
Use the `calculate_tax_base` tool. You provide the net product value and the tax rate, and it returns the grossed-up base and the tax amount included in that base.

**Q: Can I calculate ICMS-ST with MVA?**
Yes. The `calculate_icms_substitution` tool allows you to input the initial tax base, the MVA percentage, and the relevant interstate and internal rates to find the substitution amount.

**Q: How does the tool determine the interstate rate?**
The `get_interstate_rate` tool checks the origin and destination regions. It applies 4% for imports, 7% for movements from South/Southeast to North/Northeast/Midwest, and 12% for all other interstate routes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/icms-calculator](https://vinkius.com/mcp/icms-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ICMS Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `icms-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ICMS Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "icms-calculator": {
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
