# Lime Requirement Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lime-requirement-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate precise limestone dosage and total application costs using base saturation and SMP buffer methods.

## Description
This MCP server provides specialized agricultural tools to determine the exact amount of lime needed for soil correction. Use `calculate_base_saturation_dosage` to calculate requirements based on current and target base saturation (V%), soil CTC, and lime PRNT. You can also use `calculate_smp_dosage` to assess needs via the SMP buffer method, and `calculate_total_expenditure` to project total mass needed and financial investment for a specific field area.


## Available Tools
- **calculate_base_saturation_dosage**: Calculates the amount of lime required to reach a desired base saturation level
- **calculate_smp_dosage**: Determines the lime requirement based on the SMP buffer capacity measurements
- **calculate_total_expenditure**: Estimates the total financial investment required for a specific field area


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lime Requirement Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate lime dosage for a soil with 40% V%, target 65%, CTC of 10, and PRNT of 85%."

**🤖 AI Agent:**
> The `calculate_base_saturation_dosage` tool would calculate the required dosage based on these parameters.

---

**👤 You:**
> "What is the cost for 50 hectares if I need 2 tonnes per hectare at $150 per tonne?"

**🤖 AI Agent:**
> Using `calculate_total_expenditure`, the total mass needed is 100 tonnes, with a total cost of $15,000.

---

**👤 You:**
> "Determine lime needs using SMP value of 4.5 and target of 6.0."

**🤖 AI Agent:**
> The `calculate_smp_dosage` tool will compute the necessary dosage per hectare to reach the target equilibrium.


## ❓ FAQ

**Q: What is the base saturation method?**
It calculates lime dosage by finding the difference between target and current V%, adjusted by soil CTC and lime PRNT using `calculate_base_saturation_dosage`.

**Q: How do I estimate total costs?**
Use the `calculate_total_expenditure` tool by providing your field area, dosage per hectare, and the market price per tonne.

**Q: Does it support the SMP buffer method?**
Yes, the `calculate_smp_dosage` tool allows you to determine lime requirements based on current and target SMP buffer values.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lime-requirement-calculator](https://vinkius.com/mcp/lime-requirement-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lime Requirement Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `lime-requirement-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lime Requirement Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lime-requirement-calculator": {
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
