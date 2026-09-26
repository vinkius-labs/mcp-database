# Emergency Supply Expiry Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/emergency-supply-expiry-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate item rotation, procurement deadlines, and storage audits for emergency preparedness.

## Description
This MCP server provides a strategic management system for emergency preparedness. It automates the Earliest-Expiry-First (EEF) rotation principle to minimize waste and ensure readiness. Use `plan_rotation_and_actions` to generate a full rotation calendar and shopping deadlines, `get_inventory_status` to monitor stock levels against safety thresholds, `calculate_shopping_deadlines` to identify critical procurement dates, and `get_storage_audit_plan` to schedule physical inspections of storage locations.


## Available Tools (4)
- **calculate_shopping_deadlines**: Identifies specific dates by which new supplies must be ordered to maintain continuous readiness
- **get_inventory_status**: Provides a real-time summary of current stock levels against safety thresholds
- **get_storage_audit_plan**: Creates a schedule for physical inspections of storage locations
- **plan_rotation_and_actions**: Generates a comprehensive management plan including usage priorities, replacement tasks, and shopping deadlines


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Emergency Supply Expiry Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a management plan for my supplies: water (qty 10, expires 2025-12-01, lead time 5 days, threshold 3), medical kit (qty 2, expires 2024-06-01, lead time 10 days, threshold 1)."

**🤖 AI Agent:**
> Your rotation plan is ready. Prioritize the medical kit for immediate use or replacement. Your shopping deadline for the medical kit is 2024-05-22 to ensure it is replaced before the June expiration.

---

**👤 You:**
> "Check the status of my inventory: water (qty 5, threshold 4), flashlight (qty 1, threshold 1)."

**🤖 AI Agent:**
> Inventory status: water is healthy, and flashlight is low.

---

**👤 You:**
> "When do I need to buy more water if it expires on 2025-01-01 and the lead time is 7 days?"

**🤖 AI Agent:**
> You must order more water by 2024-12-25 to maintain continuous readiness.


## ❓ FAQ

**Q: How does the rotation logic work?**
The system uses the Earliest-Expiry-First (EEF) rule. By using `plan_rotation_and_actions`, you receive a prioritized schedule to consume or replace items before they expire.

**Q: How can I track if my supplies are running low?**
You can use the `get_inventory_status` tool. It compares your current quantities against your defined threshold levels and flags items as healthy, low, or critical.

**Q: Can I schedule regular storage checks?**
Yes. The `get_storage_audit_plan` tool allows you to generate a recurring schedule for physical inspections of your storage locations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/emergency-supply-expiry-planner](https://vinkius.com/en/ai-agent-connect/emergency-supply-expiry-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Emergency Supply Expiry Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emergency-supply-expiry-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Emergency Supply Expiry Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emergency-supply-expiry-planner": {
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
