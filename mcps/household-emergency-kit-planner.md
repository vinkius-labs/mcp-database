# Household Emergency Kit Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-emergency-kit-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [safety](../categories/safety.md)

Generate staged supply plans, storage assignments, and renewal calendars for household emergency kits.

## Description
This MCP server provides a comprehensive management system for building and maintaining household emergency preparedness. It uses specialized tools like `get_supply_plan` to create multi-phase acquisition roadmaps that respect your budget and storage constraints. You can use `get_inventory_status` to identify supply gaps and `get_container_assignments` to organize items into physical storage units. Additionally, `get_renewal_schedule` helps you maintain your kit by tracking expiry dates for food, water, and medical supplies. It is designed to help families prepare for local risks like floods, wildfires, or power outages through organized, staged planning.


## Available Tools (4)
- **get_container_assignments**: Maps the items into physical storage containers
- **get_inventory_status**: Evaluates current stock against the requirements of the selected kit categories
- **get_renewal_schedule**: Calculates a calendar of upcoming maintenance tasks to prevent expired supplies
- **get_supply_plan**: Generates the high-level strategy for building the kit based on all user constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Emergency Kit Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a staged supply plan for a family of 4 with 2 children and a dog, living in a wildfire-prone area with a $500 budget."

**🤖 AI Agent:**
> I have generated a 3-stage plan. Stage 1 focuses on immediate water and fire-safety items ($150). Stage 2 adds medical and sanitation supplies ($200). Stage 3 completes the kit with long-term food storage ($150). Total cost is $500, fitting your budget.

---

**👤 You:**
> "Check my current inventory for gaps in a basic survival kit."

**🤖 AI Agent:**
> Based on your existing supplies, you are missing 10 liters of water and 1 first-aid kit to meet the basic survival requirements for your household.

---

**👤 You:**
> "How should I organize my emergency supplies in my available storage bins?"

**🤖 AI Agent:**
> I have assigned your items to two containers. Bin A will hold your high-priority water and food supplies, while Bin B will contain your medical and sanitation tools.


## ❓ FAQ

**Q: How does the staged supply plan work?**
The `get_supply_plan` tool breaks down the kit building process into manageable phases. It ensures you don't exceed your budget or your physical storage limits by spreading out purchases over time.

**Q: Can I manage my existing supplies?**
Yes. By using `get_inventory_status`, the system compares what you already have against the requirements for your specific risk profile and household needs, highlighting exactly what is missing.

**Q: How do I know when to replace expired items?**
The `get_renewal_schedule` tool generates a maintenance calendar. It tracks the expiry dates of your current and planned supplies so you know exactly when to rotate your stock.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-emergency-kit-planner](https://vinkius.com/en/ai-agent-connect/household-emergency-kit-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Emergency Kit Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-emergency-kit-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Emergency Kit Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-emergency-kit-planner": {
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
