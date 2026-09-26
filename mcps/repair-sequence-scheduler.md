# Repair Sequence Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-sequence-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A high-precision engine for synchronizing home repair timelines, trade dependencies, and room constraints.

## Description
The Repair Sequence Scheduler connects AI agents to complex home renovation logic. It synchronizes trade dependencies, worker availability, and physical room constraints to build optimized timelines. Use `plan_repair_schedule` to generate a complete chronological work plan and identify the critical path. You can use `calculate_homeowner_plan` to determine when you need to be present or avoid certain rooms. If a project hits a snag, `evaluate_delay_impact` predicts how a specific delay ripples through the entire schedule, while `validate_resource_constraints` ensures your proposed plan is physically possible.


## Available Tools (4)
- **calculate_homeowner_plan**: Identifies specific windows where the homeowner must be present or should avoid being present
- **evaluate_delay_impact**: Predicts how a delay in a specific task will ripple through the entire schedule
- **plan_repair_schedule**: Generates the complete chronological work plan and identifies the critical path
- **validate_resource_constraints**: Checks a proposed set of tasks against worker and room availability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair Sequence Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a repair schedule for painting a bedroom and fixing a leak, where the leak must be fixed before painting starts."

**🤖 AI Agent:**
> The schedule is set: Plumbing repair will occur on Monday, followed by the bedroom painting on Wednesday once the area is clear.

---

**👤 You:**
> "What happens to my schedule if the electrician is delayed by 2 days?"

**🤖 AI Agent:**
> A 2-day delay for the electrician will push the subsequent drywall and painting tasks back by exactly 2 days, moving the final completion date to Friday.

---

**👤 You:**
> "When should I be home to assist with the intrusive repair tasks?"

**🤖 AI Agent:**
> You should be present on Tuesday morning for the electrical inspection and avoid the kitchen on Wednesday afternoon during the floor curing phase.


## ❓ FAQ

**Q: How do I generate a full project timeline?**
You can use the `plan_repair_schedule` tool by providing the list of tasks, dependencies, worker availability, and room constraints.

**Q: Can I check if a delay will push back my deadline?**
Yes, use `evaluate_delay_impact` to see how a specific task delay affects the final completion date and which other tasks are pushed back.

**Q: How does the tool handle room conflicts?**
The engine uses `validate_resource_constraints` to ensure no two trades occupy the same room at the same time, preventing physical overlaps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-sequence-scheduler](https://vinkius.com/en/ai-agent-connect/repair-sequence-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair Sequence Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-sequence-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair Sequence Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-sequence-scheduler": {
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
