# Resin Volume Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/resin-volume-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Calculate precise resin volumes, weights, and mixing ratios for epoxy casting projects.

## Description
The Resin Volume Calculator is a precision utility designed for epoxy and resin artists. It bridges the gap between mould dimensions and the actual amount of material needed. Using tools like `calculate_mould_volume`, you can determine the capacity of rectangular, cylindrical, spherical, or irregular moulds. The `calculate_material_mass` tool allows you to convert that volume into weight based on your resin's density, while `calculate_mix_quantities` ensures you have the exact amounts of Part A and Part B required, including a safety overage buffer to prevent running short during a pour.


## Available Tools (3)
- **calculate_material_mass**: Convert volume to mass
- **calculate_mix_quantities**: Calculate resin part amounts
- **calculate_mould_volume**: Calculate the volume of a mould


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Resin Volume Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a cylindrical mould with a radius of 5cm and a depth of 10cm. How much resin do I need?"

**🤖 AI Agent:**
> The volume of your cylindrical mould is approximately 785.4 ml.

---

**👤 You:**
> "Convert 500ml of resin with a density of 1.1 g/ml to weight."

**🤖 AI Agent:**
> The total mass for 500ml of resin at 1.1 g/ml is 550 grams.

---

**👤 You:**
> "How much Part A and Part B do I need for a 2:1 ratio with a total of 300ml, including a 10% overage?"

**🤖 AI Agent:**
> Including the 10% overage, you will need 220 ml of Part A and 110 ml of Part B.


## ❓ FAQ

**Q: How do I calculate the volume for an irregular mould?**
For irregular shapes, use the water displacement method to find the volume in ml, then provide this value to the `calculate_mould_volume` tool using the 'irregular' shape setting.

**Q: Can I calculate mixing ratios by weight or volume?**
Yes, the `calculate_mix_quantities` tool supports both 'weight' and 'volume' measurement modes. You can also provide density to convert between them.

**Q: What is the recommended overage percentage?**
It is highly recommended to add a 5-10% buffer using the `overage_percentage` parameter in `calculate_mix_quantities` to account for resin lost in mixing containers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/resin-volume-calculator](https://vinkius.com/mcp/resin-volume-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Resin Volume Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `resin-volume-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Resin Volume Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "resin-volume-calculator": {
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
