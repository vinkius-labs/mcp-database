# Local Advocacy Meeting Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-advocacy-meeting-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate structured meeting agendas, speaker orders, and action plans for local advocacy.

## Description
This MCP server provides a suite of tools to organize effective local advocacy meetings. It helps organizers create chronological agendas using `generate_meeting_agenda`, determine the most impactful sequence of speakers with `optimize_speaker_order`, prepare logistical and content requirements via `create_preparation_checklist`, and transform meeting goals into actionable follow-up strategies with `draft_action_plan`. All outputs are designed to ensure factual alignment and respectful participation.


## Available Tools (4)
- **create_preparation_checklist**: Generates a list of tasks to ensure the meeting is logistically and content-ready
- **draft_action_plan**: Transforms meeting goals into a concrete follow-up strategy
- **generate_meeting_agenda**: Creates a chronological timeline of the meeting events
- **optimize_speaker_order**: Determines the most effective sequence of speakers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Advocacy Meeting Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a meeting agenda for a community discussion on local park improvements. We have 45 minutes, starting at 6:00 PM at the Community Center. Participants are Alice (Organizer) and Bob (Resident). Each speaker gets 10 minutes."

**🤖 AI Agent:**
> The meeting agenda is set for 45 minutes. It includes an introduction, 20 minutes of speaking time for Alice and Bob, and 15 minutes for community discussion and closing.

---

**👤 You:**
> "What is the best order for speakers at a meeting about new bike lanes? Participants: Sarah (Urban Planner), Mike (Local Business Owner), and Elena (Cyclist)."

**🤖 AI Agent:**
> The recommended sequence is Sarah (Urban Planner) to provide context, followed by Elena (Cyclist) for impact testimony, and Mike (Local Business Owner) to discuss local implications.

---

**👤 You:**
> "Generate a preparation checklist for a meeting about water quality. We need to use the city's annual report and ensure the venue is wheelchair accessible."

**🤖 AI Agent:**
> The checklist includes verifying the city's annual report is available for all speakers and confirming the venue's wheelchair accessibility is fully prepared.


## ❓ FAQ

**Q: How does the tool ensure the meeting stays on schedule?**
The `generate_meeting_agenda` tool calculates a timeline that respects the total duration provided, including buffers for transitions and concluding remarks.

**Q: Can I use this to organize a formal public hearing?**
Yes, the tools are designed to handle various meeting tiers, including Public Advocacy Tier meetings which require strict adherence to factual sources.

**Q: How are follow-up tasks assigned?**
The `draft_action_plan` tool decomposes meeting goals into specific tasks and assigns them to the participants provided in the input.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-advocacy-meeting-planner](https://vinkius.com/en/ai-agent-connect/local-advocacy-meeting-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Advocacy Meeting Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-advocacy-meeting-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Advocacy Meeting Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-advocacy-meeting-planner": {
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
