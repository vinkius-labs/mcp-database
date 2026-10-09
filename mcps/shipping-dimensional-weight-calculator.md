# Shipping Dimensional Weight Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/shipping-dimensional-weight-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate volumetric and billable shipping weights using carrier divisors.

## Description
This MCP server provides essential tools for logistics and shipping calculations. It allows AI agents to determine the volumetric weight of a package using `calculate_dimensional_weight` and find the final weight a carrier will charge using `calculate_billable_weight`. You can also use `validate_dimensions` to ensure package measurements are logical and `get_standard_divisors` to retrieve common industry volumetric constants.


## Available Tools (4)
- **calculate_billable_weight**: Calculate the final billable weight for a package
- **calculate_dimensional_weight**: Calculate the volumetric weight of a package
- **get_standard_divisors**: Get standard carrier divisors
- **validate_dimensions**: Validate package dimensions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shipping Dimensional Weight Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the volumetric weight for a package that is 10x12x15 inches with a divisor of 166?"

**🤖 AI Agent:**
> The dimensional weight for the package is 10.84.

---

**👤 You:**
> "A package is 20x20x20 inches, weighs 10 lbs, and the divisor is 139. What is the billable weight?"

**🤖 AI Agent:**
> The dimensional weight is 57.55, and since this is greater than the actual weight of 10 lbs, the billable weight is 57.55.

---

**👤 You:**
> "Are dimensions of 5, 5, and -2 valid?"

**🤖 AI Agent:**
> No, the dimensions are not valid because one of the values is negative.


## ❓ FAQ

**Q: What is dimensional weight?**
Dimensional weight is a theoretical weight calculated from a package's volume and a carrier's specific divisor.

**Q: How is billable weight determined?**
The billable weight is the higher value between the package's actual physical weight and its calculated dimensional weight.

**Q: Can I get standard carrier divisors?**
Yes, you can use the `get_standard_divisors` tool to retrieve common domestic and international volumetric constants.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/shipping-dimensional-weight-calculator](https://vinkius.com/en/ai-agent-connect/shipping-dimensional-weight-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shipping Dimensional Weight Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shipping-dimensional-weight-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shipping Dimensional Weight Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shipping-dimensional-weight-calculator": {
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
