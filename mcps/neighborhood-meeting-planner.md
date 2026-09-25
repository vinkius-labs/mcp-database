# Neighborhood Meeting Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/neighborhood-meeting-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate structured meeting agendas, venue selections, and community invitations.

## Description
This MCP server provides a complete toolkit for organizing community gatherings. Use `plan_meeting` to automatically select viable venues based on budget and accessibility, while ensuring the agenda respects time constraints and priority levels. It also includes tools to `generate_invitation` for professional community outreach and `generate_decision_template` to ensure all meeting outcomes are recorded according to your chosen consensus rules.


## Available Tools (4)
- **generate_decision_template**: Creates a structured template for recording outcomes and decisions made during the meeting
- **generate_invitation**: Produces professional invitation text tailored to the meeting details
- **plan_meeting**: Generates a comprehensive meeting plan including a timeline, venue selection, and facilitator assignments
- **validate_scheduling**: Checks if a proposed meeting date is feasible based on notice requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Neighborhood Meeting Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Help me plan a neighborhood meeting for 20 people with a $100 budget. We need wheelchair access. Topics: 'Park Cleanup' (Priority 1, 30 mins) and 'Safety Update' (Priority 2, 20 mins)."

**🤖 AI Agent:**
> The meeting plan is ready. The Community Center has been selected as it meets the $100 budget and provides wheelchair access. The agenda will address 'Park Cleanup' first, followed by 'Safety Update', totaling 50 minutes.

---

**👤 You:**
> "Generate an invitation for a meeting titled 'Summer Festival Planning' on July 15th at 6 PM at the Library."

**🤖 AI Agent:**
> Subject: Invitation: Summer Festival Planning Meeting

Dear Neighbors,

Please join us for the Summer Festival Planning meeting on July 15th at 6 PM at the Library. We will be discussing the upcoming festival details.

---

**👤 You:**
> "Is it okay to schedule a meeting for tomorrow if I am planning it today and need 3 days notice?"

**🤖 AI Agent:**
> No, the proposed date is not feasible because it does not meet the required 3-day notice period.


## ❓ FAQ

**Q: How does the tool select a venue?**
The `plan_meeting` tool filters available venues by capacity, budget, and required accessibility features to find the best fit for your attendees.

**Q: Can I customize the meeting invitation?**
Yes, by using `generate_invitation`, you can produce professional text tailored to your specific meeting title, location, and agenda.

**Q: How are decisions recorded?**
You can use `generate_decision_template` to create a structured record that captures the decision reached, the voting outcome, and the proponents for each topic.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/neighborhood-meeting-planner](https://vinkius.com/en/ai-agent-connect/neighborhood-meeting-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Neighborhood Meeting Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `neighborhood-meeting-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Neighborhood Meeting Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "neighborhood-meeting-planner": {
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
