# Shipping Charge Totalizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/shipping-charge-totalizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Aggregates and validates shipping fees to calculate total logistics costs.

## Description
This MCP server provides specialized tools for managing shipping logistics. It allows AI agents to perform precise calculations such as `calculate_total_shipping` to sum multiple fees, `validate_charge_format` to ensure individual amounts are non-negative, and `filter_valid_charges` to clean datasets. It also includes `get_average_shipping_cost` to determine mean costs across shipments. These tools help in determining shipping tiers and ensuring mathematical accuracy in logistics workflows.


## Available Tools (4)
- **get_average_shipping_cost**: Calculate the mean shipping cost among the provided charges
- **calculate_total_shipping**: Calculate the total sum of all provided shipping charges
- **filter_valid_charges**: Filter a list of charges to find legitimate non-negative values
- **validate_charge_format**: Validate if a specific value is a valid shipping charge


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shipping Charge Totalizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total sum of these shipping charges: 10.50, 5.00, and 2.25?"

**🤖 AI Agent:**
> The total sum of the shipping charges is 17.75.

---

**👤 You:**
> "Is -5.00 a valid shipping charge?"

**🤖 AI Agent:**
> No, -5.00 is not a valid shipping charge because charges must be non-negative.

---

**👤 You:**
> "Filter the valid charges from this list: 12.00, -3.00, 8.50, -1.00."

**🤖 AI Agent:**
> The valid charges are 12.00 and 8.50.


## ❓ FAQ

**Q: How can I sum multiple shipping fees?**
You can use the `calculate_total_shipping` tool by providing a list of charge amounts.

**Q: Does this tool support negative values?**
No, shipping charges must be non-negative. The `validate_charge_format` tool can be used to verify if a value is valid.

**Q: Can I find the average cost of my shipments?**
Yes, the `get_average_shipping_cost` tool calculates the mean cost from a provided list of charges.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/shipping-charge-totalizer](https://vinkius.com/en/ai-agent-connect/shipping-charge-totalizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shipping Charge Totalizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shipping-charge-totalizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shipping Charge Totalizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shipping-charge-totalizer": {
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
