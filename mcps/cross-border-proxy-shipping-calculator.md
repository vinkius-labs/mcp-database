# Cross-Border Proxy Shipping Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/cross-border-proxy-shipping-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [e-commerce](../categories/e-commerce.md)

Calculate volumetric weight and shipping costs for China-Japan proxy services.

## Description
This MCP server provides precise shipping calculations for proxy services operating between China and Japan. It determines the volumetric weight based on package dimensions and the selected shipping method, calculates the final billable weight by rounding up to the nearest 0.5 kg, and estimates the total shipping cost in JPY. Use `calculate_shipping_metrics` to find the weight used for billing and `estimate_shipping_cost` to get the final price.


## Available Tools (3)
- **calculate_shipping_metrics**: Calculate volumetric and billable weight for a package
- **estimate_shipping_cost**: Estimate the shipping cost in JPY
- **get_shipping_method_info**: Get information about a shipping method


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cross-Border Proxy Shipping Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the billable weight for a 2kg package that is 30x30x30 cm using EMS?"

**🤖 AI Agent:**
> The volumetric weight is 4.5 kg, so the billable weight is 4.5 kg.

---

**👤 You:**
> "How much will it cost to ship a 5kg package via Sea shipping?"

**🤖 AI Agent:**
> The estimated shipping cost for 5kg via Sea is 2500 JPY.

---

**👤 You:**
> "Get info about the SAL shipping method."

**🤖 AI Agent:**
> SAL is an Economy service that uses a divisor of 8000 for volumetric calculations.


## ❓ FAQ

**Q: How is volumetric weight calculated?**
Volumetric weight is calculated by dividing the package volume by 6000 for EMS/DHL or 8000 for SAL/Sea.

**Q: What is billable weight?**
Billable weight is the higher of the actual weight or the volumetric weight, rounded up to the nearest 0.5 kg.

**Q: Can I use this for DHL shipments?**
Yes, you can use `estimate_shipping_cost` to calculate costs for DHL using the appropriate weight metrics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/cross-border-proxy-shipping-calculator](https://vinkius.com/ai-agent-connect/cross-border-proxy-shipping-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cross-Border Proxy Shipping Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cross-border-proxy-shipping-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cross-Border Proxy Shipping Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cross-border-proxy-shipping-calculator": {
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
