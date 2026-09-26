# Household Utility Handover Sheet MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-utility-handover-sheet)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate structured handover documentation and synchronized task lists for utility transitions.

## Description
This MCP server facilitates the formal transfer of domestic services like electricity, water, and gas between residents. It uses `generate_handover_summary` to consolidate service statuses, `create_responsibility_matrix` to assign liability, and `generate_task_lists` to produce dated schedules for both incoming and outgoing parties. You can also use `validate_handover_completeness` to ensure all meter readings and assignments are captured to prevent billing disputes.


## Available Tools (4)
- **generate_task_lists**: Produces two distinct, dated schedules of actions--one for the Incoming Party and one for the Outgoing Party
- **create_responsibility_matrix**: Explicitly defines which party is responsible for which service and the contact information for the relevant account holders
- **generate_handover_summary**: Creates a comprehensive overview of all utility services and their current status at the point of handover
- **validate_handover_completeness**: An audit tool to check if all necessary data points are present to prevent disputed bills or missed service transfers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Utility Handover Sheet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a summary for a handover on 2024-05-15 with electricity at 1250 kWh and water at 45 m3."

**🤖 AI Agent:**
> The handover summary for 2024-05-15 is ready. Electricity is recorded at 1250 kWh and Water at 45 m3.

---

**👤 You:**
> "Create a responsibility matrix for Electricity (Outgoing) and Water (Incoming)."

**🤖 AI Agent:**
> The responsibility matrix has been created. The Outgoing party is responsible for Electricity, and the Incoming party is responsible for Water.

---

**👤 You:**
> "Generate task lists for a handover on 2024-06-01 with a task to notify the gas provider."

**🤖 AI Agent:**
> The task lists for 2024-06-01 have been generated. The Outgoing party must notify the gas provider.


## ❓ FAQ

**Q: How can I ensure billing accuracy during a move?**
Use the `generate_handover_summary` tool to record meter readings at the exact moment of handover, creating a legal snapshot for providers.

**Q: Can I generate schedules for both parties?**
Yes, the `generate_task_lists` tool produces two distinct, dated schedules--one for the Incoming Party and one for the Outgoing Party.

**Q: How do I check if my handover documentation is complete?**
You can run `validate_handover_completeness` to audit your data and identify any missing meter readings or unassigned services.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-utility-handover-sheet](https://vinkius.com/en/ai-agent-connect/household-utility-handover-sheet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Utility Handover Sheet** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-utility-handover-sheet` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Utility Handover Sheet** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-utility-handover-sheet": {
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
