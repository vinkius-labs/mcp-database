# Dimensional Weight Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dimensional-weight-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate dimensional weights, billable weight, and shipping weight discrepancies for major global carriers.

## Description
This MCP server provides essential tools for logistics professionals to manage shipping costs by calculating volumetric weights. Using the `get_all_carrier_dim_weights` tool, you can determine how much space a package occupies across carriers like FedEx, UPS, DHL, and USPS. The `resolve_billable_weight` tool helps identify the final weight used for invoicing by comparing actual mass to dimensional weight, while `calculate_weight_gap` quantifies the extra cost incurred from low-density shipments.


## Available Tools (3)
- **resolve_billable_weight**: Determates the final weight that will be charged by the carrier
- **calculate_weight_gap**: Calculates the discrepancy between actual weight and billable weight
- **get_all_carrier_dim_weights**: Returns weights for FedEx, UPS, DHL, and USPS.

Calculates the dimensional weight for all supported carriers based on dimensions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dimensional Weight Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the dimensional weight for a package that is 10x10x10 inches for FedEx?"

**🤖 AI Agent:**
> The dimensional weight for a 10x10x10 inch package via FedEx is approximately 6.94 lbs.

---

**👤 You:**
> "My package weighs 5kg, but the dimensional weight is 8kg. How much extra weight am I paying for?"

**🤖 AI Agent:**
> You are paying for an additional 3kg of weight due to the package volume.

---

**👤 You:**
> "Calculate all carrier weights for a box measuring 50x40x30 cm."

**🤖 AI Agent:**
> The dimensional weights are: FedEx: 5.39, UPS: 5.39, DHL: 5.39, and USPS: 4.32.


## ❓ FAQ

**Q: Which carriers are supported?**
The server supports FedEx, UPS, DHL, and USPS.

**Q: How is the dimensional weight calculated?**
It calculates the volume of the package and divides it by a carrier-specific divisor (e.g., 139 for FedEx/UPS/DHL, 166 for USPS).

**Q: What is billable weight?**
Billable weight is the higher value between the package's actual physical mass and its calculated dimensional weight.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dimensional-weight-calculator](https://vinkius.com/mcp/dimensional-weight-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dimensional Weight Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dimensional-weight-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dimensional Weight Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dimensional-weight-calculator": {
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
