# US Building Permit Fee Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-building-permit-fee-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Estimate building permit, plan check, and inspection fees for major US cities.

## Description
This MCP server provides precise estimates for construction-related fees including permit costs, plan check fees, and inspection charges. By using tools like `estimate_permit_fee`, `lookup_city_rules`, and `verify_valuation`, users can instantly calculate potential municipal expenses based on project valuation for cities such as New York City, Los Angeles, Chicago, Houston, and Phoenix.


## Available Tools (3)
- **estimate_permit_fee**: Calculate estimated building permit fees
- **lookup_city_rules**: Lookup fee rules for a specific city
- **verify_valuation**: Verify if a valuation is valid for a city


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Building Permit Fee Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will it cost to get a permit in New York City for a project valued at $500,000?"

**🤖 AI Agent:**
> For a construction valuation of $500,000 in New York City, the estimated permit fee is $12,500, with a plan check fee of $2,500 and inspection fees totaling $1,200.

---

**👤 You:**
> "Check if a $10,000 valuation is valid for Los Angeles."

**🤖 AI Agent:**
> Yes, a valuation of $10,000 is valid for Los Angeles; it meets the minimum requirements for permit processing.

---

**👤 You:**
> "What are the fee rules for Chicago?"

**🤖 AI Agent:**
> In Chicago, plan check fees are calculated based on a percentage of the construction valuation, and inspection fees follow a standard base rate structure.


## ❓ FAQ

**Q: How accurate are the fee estimates?**
Estimates are based on hardcoded municipal fee schedules. While highly accurate for the provided data, always verify with the local building department before finalizing budgets.

**Q: Which cities are supported?**
Currently, the server supports major US municipalities including New York City, Los Angeles, Chicago, Houston, and Phoenix.

**Q: What does 'construction valuation' mean?**
Construction valuation is the total estimated cost of all work related to the permit, including both materials and labor.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-building-permit-fee-estimator](https://vinkius.com/mcp/us-building-permit-fee-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Building Permit Fee Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-building-permit-fee-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Building Permit Fee Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-building-permit-fee-estimator": {
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
