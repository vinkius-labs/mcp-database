# US Corporate Tax Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-corporate-tax-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Estimate US federal and state corporate income taxes, providing comparative analysis between C-Corp, S-Corp, and LLC structures.

## Description
This MCP server provides a specialized calculation engine for estimating US corporate tax liabilities. It allows AI agents to retrieve state-specific tax rates using `get_state_tax_rate`, calculate detailed federal and state tax breakdowns with `calculate_tax_liability`, and perform complex comparative analyses between different business entities like C-Corp, S-Corp, and LLC via `compare_business_structures`. The tool accounts for the 21% flat federal rate and applies hardcoded state-level corporate income tax rates to provide an accurate effective tax rate estimation.


## Available Tools (3)
- **calculate_tax_liability**: Calculates the specific tax breakdown for a single profit amount in a given state
- **compare_business_structures**: Provides a side-by-side comparison of tax burdens for different business structures
- **get_state_tax_rate**: Retrieves the hardcoded corporate income tax rate for a specific US state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Corporate Tax Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the corporate tax rate in California?"

**🤖 AI Agent:**
> The tool `get_state_tax_rate` can be used with 'CA' to retrieve the current hardcoded rate.

---

**👤 You:**
> "Calculate the tax liability for a $500,000 profit in Texas."

**🤖 AI Agent:**
> Using `calculate_tax_liability` with a profit of 500000 and stateCode 'TX' will provide the federal, state, and total tax breakdown.

---

**👤 You:**
> "Compare C-Corp vs LLC for a $1,000,000 profit in New York."

**🤖 AI Agent:**
> The `compare_business_structures` tool will analyze the tax implications for C-Corp, S-Corp, and LLC based on the $1,000,000 profit in NY.


## ❓ FAQ

**Q: How can I find the tax rate for a specific state?**
You can use the `get_state_tax_rate` tool by providing the two-letter US state abbreviation (e.g., 'NY' for New York).

**Q: Does this tool calculate federal taxes?**
Yes. The `calculate_tax_liability` tool calculates both the 21% federal corporate tax and the applicable state-level tax.

**Q: Can I compare different business structures?**
Yes, the `compare_business_structures` tool provides a side-by-side comparison of tax burdens for C-Corp, S-Corp, and LLC entities.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-corporate-tax-calculator](https://vinkius.com/mcp/us-corporate-tax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Corporate Tax Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-corporate-tax-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Corporate Tax Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-corporate-tax-calculator": {
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
