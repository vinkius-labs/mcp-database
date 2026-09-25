# Care Visit Coordination Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-visit-coordination-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transforms care goals and logistical constraints into actionable visit schedules and checklists.

## Description
This MCP server provides a professional planning system for care coordination. It uses `generate_visit_schedule` to create chronological timelines, `create_preparation_checklist` to prepare helpers for arrival, `calculate_contact_sequence` to manage caregiver notifications, and `get_post_visit_template` to ensure consistent reporting. It manages visit spacing, access protocols, and handoff logic to ensure continuity of care.


## Available Tools (4)
- **calculate_contact_sequence**: Determines the order and method of notifying parties involved in the care plan
- **create_preparation_checklist**: Generates a list of items and steps a helper needs to complete before arriving at a visit
- **generate_visit_schedule**: Creates a chronological timeline of visits based on goals, available times, and spacing rules
- **get_post_visit_template**: Provides a structured format for helpers to record what happened during the visit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Visit Coordination Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a visit schedule for these goals: physical therapy, with these available times: ["2024-07-01T10:00:00Z", "2024-07-01T14:00:00Z"], and this helper availability: ["helper_1"]."

**🤖 AI Agent:**
> The visit for physical therapy is scheduled for 2024-07-01 from 10:00 AM to 11:00 AM, assigned to helper_1.

---

**👤 You:**
> "Generate a preparation checklist for the scheduled visit with access instructions: 'Gate code 1234'."

**🤖 AI Agent:**
> Your checklist: 1. Verify gate code 1234. 2. Confirm arrival time.

---

**👤 You:**
> "What is the contact sequence for the upcoming visit at 2 PM?"

**🤖 AI Agent:**
> The notification order is: 1. Primary Caregiver (High Priority), 2. Secondary Contact (Medium Priority).


## ❓ FAQ

**Q: How does the scheduling work?**
The `generate_visit_schedule` tool calculates visit times by applying spacing requirements and helper availability to the provided time windows.

**Q: Can I generate a checklist for my helpers?**
Yes, using `create_preparation_checklist`, you can generate actionable steps including access instructions and transport needs.

**Q: How is privacy handled during reporting?**
The `get_post_visit_template` tool uses your specified privacy preferences to filter what details are recorded in the final report.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-visit-coordination-plan](https://vinkius.com/en/ai-agent-connect/care-visit-coordination-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Visit Coordination Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-visit-coordination-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Visit Coordination Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-visit-coordination-plan": {
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
