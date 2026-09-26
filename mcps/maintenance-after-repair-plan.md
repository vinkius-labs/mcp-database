# Maintenance After Repair Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/maintenance-after-repair-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [asset-management](../categories/asset-management.md)

Generates structured maintenance schedules and inspection checklists for assets following a repair.

## Description
This MCP server provides specialized planning tools for the lifecycle of an asset immediately following a repair. It uses `generate_maintenance_plan` to create structured maintenance packages, `get_inspection_checklist` to identify physical indicators of repair success, `calculate_next_service_window` to determine intervention timing, and `query_material_care_rules` to retrieve baseline material requirements. The system integrates manufacturer instructions and climate exposure to provide precise, actionable maintenance calendars.


## Available Tools (4)
- **query_material_care_rules**: Retrieves baseline care requirements for specific materials
- **calculate_next_service_window**: Determines the exact timing for the next required intervention
- **generate_maintenance_plan**: Creates the complete structured maintenance package for a post-repair asset
- **get_inspection_checklist**: Provides a focused list of physical indicators to ensure repair success


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Maintenance After Repair Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a maintenance plan for a structural reinforcement repair using galvanized steel in a coastal environment with these instructions: [{'taskName': 'Corrosion Check', 'intervalMonths': 6, 'description': 'Inspect for rust'}]"

**🤖 AI Agent:**
> Your maintenance plan for the structural reinforcement is ready. Recurring tasks include a Corrosion Check every 3 months due to coastal exposure. Inspection signs to watch for include surface discoloration and pitting on the galvanized steel. Your next service window is scheduled for June 2024.

---

**👤 You:**
> "What are the inspection signs for a sealing repair using silicone in a temperate climate?"

**🤖 AI Agent:**
> For a silicone sealing repair, you should monitor for adhesion loss, surface cracking, or material shrinkage.

---

**👤 You:**
> "When is my next service due if my last service was 2023-10-01 and the manufacturer recommends every 12 months in an arid climate?"

**🤖 AI Agent:**
> Your next service is due on 2024-10-01. The urgency level is Low.


## ❓ FAQ

**Q: How does the plan account for environmental factors?**
The system uses the `climateExposure` input to adjust the frequency of tasks and service windows, ensuring higher-risk environments like Coastal areas receive more frequent inspections.

**Q: Can I use my own manufacturer instructions?**
Yes, you can provide specific manufacturer instructions via the `generate_maintenance_plan` tool to ensure the schedule adheres to official guidelines.

**Q: What information is needed to generate a plan?**
To use `generate_maintenance_plan`, you need the repair type, a list of installed materials, manufacturer instructions, and the climate exposure context.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/maintenance-after-repair-plan](https://vinkius.com/en/ai-agent-connect/maintenance-after-repair-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Maintenance After Repair Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `maintenance-after-repair-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Maintenance After Repair Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "maintenance-after-repair-plan": {
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
