# Household Recovery Orchestrator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-recovery-orchestrator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Converts post-disaster property data into actionable recovery sequences and schedules.

## Description
This MCP server provides a strategic orchestration engine for post-disaster recovery. It processes official re-entry guidance and property status to generate a prioritized `get_recovery_sequence`. It also manages logistics through `generate_booking_calendar`, organizes insurance documentation via `compile_evidence_list`, and coordinates family updates with `create_communication_plan`.


## Available Tools (4)
- **generate_booking_calendar**: Creates a conflict-free schedule for service providers and household members
- **get_recovery_sequence**: Generates a prioritized list of tasks required to restore the household
- **compile_evidence_list**: Aggregates all necessary documentation and observations for insurance purposes
- **create_communication_plan**: Drafts a schedule of updates for the family based on task progress


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Recovery Orchestrator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a recovery sequence for a house where authorities have permitted re-entry, but there is minor water damage."

**🤖 AI Agent:**
> 1. Safety Inspection, 2. Water Extraction, 3. Dehumidification, 4. Structural Assessment, 5. Cleaning.

---

**👤 You:**
> "Create a booking calendar for a plumber visiting tomorrow at 10 AM and a family member available all day."

**🤖 AI Agent:**
> Confirmed: Plumber appointment at 10:00 AM. No conflicts detected with household availability.

---

**👤 You:**
> "Compile an evidence list based on photos of broken windows and an existing insurance policy."

**🤖 AI Agent:**
> Visual Evidence: Photos of broken windows (High Priority). Administrative Evidence: Insurance Policy (Required).


## ❓ FAQ

**Q: How does the tool handle safety hazards?**
The `get_recovery_sequence` tool applies a strict no-hazardous-access boundary. If structural or electrical hazards are detected, all recovery tasks are blocked.

**Q: Can I use this to organize insurance claims?**
Yes, you can use `compile_evidence_list` to aggregate observed property status and document records into a prioritized registry for your insurer.

**Q: How are service appointments managed?**
The `generate_booking_calendar` tool creates a conflict-free schedule by mapping professional service appointments against household availability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-recovery-orchestrator](https://vinkius.com/en/ai-agent-connect/household-recovery-orchestrator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Recovery Orchestrator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-recovery-orchestrator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Recovery Orchestrator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-recovery-orchestrator": {
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
