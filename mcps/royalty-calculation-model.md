# Royalty Calculation Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/royalty-calculation-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates oil and gas royalty payments using jurisdictional rules.

## Description
This MCP server provides precise tools for calculating oil and gas royalties. It handles both Royalty-in-Value (RIV) and Royalty-in-Kind (RIK) models. Users can use `calculate_royalty_value` to determine cash payments based on production volume, market price, and specific jurisdictional deduction rules. The `calculate_royalty_kind` tool calculates physical product volumes, while `get_jurisdiction_rules` provides regulatory parameters for different regions. All inputs can be verified using `validate_production_data` to ensure mathematical consistency before processing.


## Available Tools (4)
- **calculate_royalty_value**: Calculates the cash amount (Royalty-in-Value) owed to a royalty owner
- **get_jurisdiction_rules**: Retrieves the specific calculation parameters and deduction rules for a given region
- **validate_production_data**: Ensures that a set of production and pricing inputs are mathematically and logically consistent
- **calculate_royalty_kind**: Calculates the physical volume of product owed to a royalty owner under a Royalty-in-Kind agreement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Royalty Calculation Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the cash royalty for 10,000 barrels at $75 per barrel with a 12.5% royalty rate in the Standard US jurisdiction, including $500 in deductions."

**🤖 AI Agent:**
> The royalty value is $89,062.50.

---

**👤 You:**
> "What is the physical volume for a 5% royalty on 50,000 cubic feet of gas?"

**🤖 AI Agent:**
> The royalty volume is 2,500 cubic feet.

---

**👤 You:**
> "Get the rules for the European/Offshore jurisdiction."

**🤖 AI Agent:**
> The European/Offshore jurisdiction allows deductions and follows value-based royalty rules.


## ❓ FAQ

**Q: What is the difference between RIV and RIK?**
Royalty-in-Value (RIV) is a cash payment based on the value of the resource, whereas Royalty-in-Kind (RIK) is the delivery of a physical portion of the produced resource.

**Q: How are deductions handled?**
Deductions are applied based on the specific jurisdiction rules retrieved via `get_jurisdiction_rules`. The logic determines if allowances are subtracted from gross value or volume.

**Q: Can I validate my data before calculating?**
Yes, you can use the `validate_production_data` tool to check if your production volume, market price, and royalty rate are logically consistent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/royalty-calculation-model](https://vinkius.com/en/ai-agent-connect/royalty-calculation-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Royalty Calculation Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `royalty-calculation-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Royalty Calculation Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "royalty-calculation-model": {
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
