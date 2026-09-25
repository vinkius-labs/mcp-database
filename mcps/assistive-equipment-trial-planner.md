# Assistive Equipment Trial Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/assistive-equipment-trial-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Coordinate and manage assistive technology trials with structured schedules and checklists.

## Description
This MCP server provides a professional management framework for coordinating the testing of assistive technology. It helps users and clinicians manage the entire trial lifecycle--from initial scheduling to final purchase decisions. Use `generate_trial_schedule` to create timelines, `create_task_checklist` to map activities to environments, and `get_observation_template` to record real-time performance data. It also includes tools like `prepare_decision_meeting_agenda` to facilitate final evaluations and `get_supplier_communication_steps` to manage vendor interactions.

### Available Tools

`generate_trial_schedule_tool`, `create_task_checklist_tool`, `get_observation_template_tool`, `prepare_decision_meeting_agenda_tool`, `get_supplier_communication_steps_tool`


## Available Tools (5)
- **create_task_checklist_tool**: Generates a structured list of activities to be performed during the trial
- **generate_trial_schedule_tool**: Creates a chronological timeline of the trial process
- **get_observation_template_tool**: Produces a standardized format for recording real-time data during the trial
- **get_supplier_communication_steps_tool**: Provides the necessary sequence of actions to interact with the vendor
- **prepare_decision_meeting_agenda_tool**: Outlines the formal meeting required to decide the fate of the equipment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Assistive Equipment Trial Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a 14-day trial schedule for a motorized wheelchair that must be returned by October 20th."

**🤖 AI Agent:**
> The trial for the motorized wheelchair will start today and run for 14 days, concluding on October 20th to meet your supplier return deadline.

---

**👤 You:**
> "Generate a task checklist for testing a walker in a home environment with success criteria of stability and ease of use."

**🤖 AI Agent:**
> The checklist includes walking through hallways, navigating doorways, and using stairs, all evaluated against stability and ease of use metrics.

---

**👤 You:**
> "I need to prepare for a meeting to decide if we should keep the new grab bars. The attendees are the primary user and an occupational therapist."

**🤖 AI Agent:**
> The decision meeting agenda is ready, focusing on comparing trial observations against the stability and grip success criteria with the primary user and therapist.


## ❓ FAQ

**Q: How do I create a testing timeline?**
You can use the `generate_trial_schedule` tool by providing the equipment name, the intended duration in days, and the supplier's return deadline. Tools available: `generate_trial_schedule_tool`, `create_task_checklist_tool`, `get_observation_template_tool`.

**Q: Can I use this to record observations during a trial?**
Yes, the `get_observation_template` tool generates a standardized format for recording qualitative notes and quantitative scores for specific tasks.

**Q: How do I handle communication with the equipment supplier?**
The `get_supplier_communication_steps` tool provides a sequence of actions for requesting trial extensions or initiating equipment returns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/assistive-equipment-trial-planner](https://vinkius.com/en/ai-agent-connect/assistive-equipment-trial-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Assistive Equipment Trial Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `assistive-equipment-trial-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Assistive Equipment Trial Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "assistive-equipment-trial-planner": {
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
