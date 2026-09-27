# Multi-Trade Repair Coordinator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/multi-trade-repair-coordinator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Synchronize construction trades with dependency sequencing and room allocation.

## Description
This MCP server acts as a central scheduling engine for complex repair and construction projects. It resolves logical dependencies between trades, manages material arrival constraints, and ensures no spatial conflicts occur by enforcing room allocation rules. Use `generate_master_schedule` to create a conflict-free timeline, `get_handoff_notes` to manage transitions between trades, `get_owner_decisions` to track critical approval points, and `get_delay_response_playbook` to recalculate schedules when disruptions occur.


## Available Tools (4)
- **get_delay_response_playbook**: Provides a recovery plan when a specific event disrupts the timeline
- **generate_master_schedule**: Produces the complete, conflict-free timeline for all requested trades and tasks
- **get_handoff_notes**: Extracts specific instructions and requirements passed from one trade to the next
- **get_owner_decisions**: Identifies critical decision points where a project owner must approve work or budget


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Multi-Trade Repair Coordinator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a master schedule for my electrical and plumbing tasks."

**🤖 AI Agent:**
> The master schedule has been generated. Electrical work is scheduled for Monday, followed by plumbing on Wednesday once the prerequisites are met.

---

**👤 You:**
> "What are the handoff requirements between the carpenter and the painter?"

**🤖 AI Agent:**
> The carpenter must complete all sanding and surface preparation before the painter can begin the first coat.

---

**👤 You:**
> "The tile delivery is delayed by 3 days. How does this affect my schedule?"

**🤖 AI Agent:**
> The 3-day delay in tile arrival pushes the flooring installation and subsequent grouting tasks back by exactly 3 days.


## ❓ FAQ

**Q: How does the tool handle room conflicts?**
The `generate_master_schedule` tool applies spatial constraints to ensure only one trade occupies a specific room at any given time.

**Q: What happens if a material delivery is late?**
You can use `get_delay_response_playbook` to receive an impact assessment and a revised schedule based on the delay.

**Q: Can I track budget-related decisions?**
Yes, `get_owner_decisions` identifies critical dates where budget milestones or inspections require owner approval.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/multi-trade-repair-coordinator](https://vinkius.com/en/ai-agent-connect/multi-trade-repair-coordinator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Multi-Trade Repair Coordinator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `multi-trade-repair-coordinator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Multi-Trade Repair Coordinator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "multi-trade-repair-coordinator": {
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
