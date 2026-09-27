# Kitchen Repair Disruption Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/kitchen-repair-disruption-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Manage household logistics during kitchen renovations with precise disruption calendars and meal planning.

## Description
This MCP server provides essential operational logistics for households undergoing kitchen repairs. It helps users navigate outages by generating a `get_disruption_calendar` to track contractor visits, a `get_temporary_kitchen_checklist` for essential supplies, a `get_delivery_coordination_plan` to prevent food spoilage, and a `get_restoration_sequence` to transition back to full functionality. It bridges the gap between construction schedules and daily household needs.


## Available Tools (4)
- **get_delivery_coordination_plan**: Synchronizes food deliveries with the renovation timeline
- **get_disruption_calendar**: Provides a chronological view of how the renovation impacts daily life
- **get_restoration_sequence**: Outlines the steps to transition from the temporary setup back to full kitchen functionality
- **get_temporary_kitchen_checklist**: Generates a list of necessary items and setup steps to maintain household function


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kitchen Repair Disruption Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a 3-day plumbing repair starting tomorrow. We are a family of 4. Our fridge is working, but the sink is out. Help me plan."

**🤖 AI Agent:**
> I have generated your disruption calendar, a temporary kitchen checklist including extra water and disposable plates for 4 people, and a delivery plan that prioritizes fresh food while your fridge is still functional.

---

**👤 You:**
> "What should I do to prepare for a full kitchen remodel where all appliances will be offline?"

**🤖 AI Agent:**
> You should use the `get_temporary_kitchen_checklist` to identify secondary cooking locations and the `get_delivery_coordination_plan` to manage food deliveries without refrigeration access.

---

**👤 You:**
> "The renovation is finished. How do I get my kitchen back to normal?"

**🤖 AI Agent:**
> The `get_restoration_sequence` will provide a step-by-step guide for cleaning, utility testing, and transitioning from your temporary setup back to full kitchen use.


## ❓ FAQ

**Q: How does this help during a renovation?**
It provides structured plans for meals, food storage, and contractor coordination to minimize daily disruption.

**Q: Can I use this for small plumbing repairs?**
Yes, the `get_disruption_calendar` tool can be used for any scope of work, from minor plumbing to full remodels.

**Q: What if my fridge is unavailable?**
The `get_delivery_coordination_plan` will detect the lack of refrigeration and suggest immediate consumption windows to prevent waste.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/kitchen-repair-disruption-planner](https://vinkius.com/en/ai-agent-connect/kitchen-repair-disruption-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kitchen Repair Disruption Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kitchen-repair-disruption-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kitchen Repair Disruption Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kitchen-repair-disruption-planner": {
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
