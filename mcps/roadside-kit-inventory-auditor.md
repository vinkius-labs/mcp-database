# Roadside Kit Inventory Auditor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/roadside-kit-inventory-auditor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automotive](../categories/automotive.md)

Audits roadside emergency kits for missing or expired items and calculates replacement costs.

## Description
This MCP server provides tools to evaluate the safety and readiness of roadside emergency kits. It identifies missing supplies, detects expired items based on a provided audit date, and calculates the total replacement cost to restore compliance. Use `audit_kit_compliance` for a full report or `get_kit_summary` for a high-level health score.


## Available Tools (4)
- **audit_kit_compliance**: Performs a complete audit of a kit to identify gaps in safety and readiness
- **calculate_total_kit_cost**: Determines the total value of all items currently inside the kit
- **check_item_availability**: Checks if a specific required item is present and valid within the inventory
- **get_kit_summary**: Provides a high-level overview of the kit's health


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Roadside Kit Inventory Auditor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Audit my roadside kit: inventory is [{'name': 'First Aid Kit', 'quantity': 1, 'expiryDate': '2025-01-01'}, {'name': 'Flashlight', 'quantity': 0, 'expiryDate': '2024-01-01'}], requirements are [{'name': 'First Aid Kit', 'minQuantity': 1, 'unitPrice': 20.0}, {'name': 'Flashlight', 'minQuantity': 1, 'unitPrice': 15.0}], auditDate is '2024-06-01'."

**🤖 AI Agent:**
> The audit is complete. Missing items: Flashlight (1 required, cost $15.0). Expired items: Flashlight (current quantity 0, cost $15.0). Total replacement cost: $15.0.

---

**👤 You:**
> "What is the total value of my current kit? Inventory: [{'name': 'Jumper Cables', 'quantity': 1}, {'name': 'Reflective Vest', 'quantity': 2}]. Price catalog: [{'name': 'Jumper Cables', 'unitPrice': 30.0}, {'name': 'Reflective Vest', 'unitPrice': 10.0}]."

**🤖 AI Agent:**
> The total inventory value is $50.0.

---

**👤 You:**
> "Is the 'Fire Extinguisher' in my kit? Inventory: [{'name': 'Fire Extinguisher', 'quantity': 1, 'expiryDate': '2023-01-01'}]. Audit date: '2024-01-01'."

**🤖 AI Agent:**
> The status of the Fire Extinguisher is expired.


## ❓ FAQ

**Q: How do I check if my roadside kit is compliant?**
You can use the `audit_kit_compliance` tool by providing your current inventory, the required items list, and the current date.

**Q: Can I calculate the cost to fix my kit?**
Yes, the `audit_kit_compliance` tool automatically calculates the total replacement cost for all missing and expired items.

**Q: What is a health score?**
The health score is a percentage provided by `get_kit_summary` that represents the ratio of present and valid items to the total required items.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/roadside-kit-inventory-auditor](https://vinkius.com/en/ai-agent-connect/roadside-kit-inventory-auditor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Roadside Kit Inventory Auditor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `roadside-kit-inventory-auditor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Roadside Kit Inventory Auditor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "roadside-kit-inventory-auditor": {
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
