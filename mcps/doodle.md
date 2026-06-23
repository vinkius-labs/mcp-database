# Doodle MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/doodle)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage group scheduling via Doodle — create meeting polls, track participant votes, handle comments, and close polls directly from any AI agent.

## Description
Connect your **Doodle** account to any AI agent and take full control of your group scheduling and meeting polls through natural conversation.

### What you can do

- **Poll Orchestration** — List all Doodle polls and retrieve explicitly attached array vectors representing titles, states (OPEN/CLOSED), and final chosen options
- **Live Poll Creation** — Provision new group scheduling polls by commanding absolute explicit text payloads for specific dates and times
- **Participant Auditing** — Enumerate explicitly attached user responses active within any target poll to identify precisely who has voted
- **Programmatic Voting** — Trigger absolute response routing to add or remove participant votes, mapping literal preference arrays (Yes, No, If-need-be) exactly
- **Collaboration Oversight** — Retrieve and append string chats and contextual comments attached to specific poll IDs to verify participant feedback
- **State Management** — Change poll states to CLOSED to lock participation arrays and override core settings to dictate finally which exact option won
- **Data Invalidation** — Irreversibly vaporize explicit poll entities and wipe all associated votes and comments from the system permanently

### How it works

1. Subscribe to this server
2. Enter your Doodle API Key (Legacy API access required, contact Doodle Enterprise for new integrations)
3. Start managing your group polls from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — coordinate meeting times across large groups and audit votes without manual follow-ups
- **Executive Assistants** — create and manage Doodle polls and monitor participant feedback using natural language
- **Operations Teams** — automate group scheduling flows and verify poll results in real-time
- **Developers** — test and debug legacy Doodle API integrations and vote mapping logic through the chat


## Available Tools (10)
- **list_polls**: Returns poll titles, states (OPEN/CLOSED), creation dates, number of participants, and chosen final options.

List all Doodle polls created by the authenticated user
- **get_poll**: Retrieve detailed information for a specific Doodle poll by ID
- **create_poll**: Participants will be invited to vote on their preferred options.

Create a new Doodle poll for group scheduling
- **delete_poll**: Drops the raw data out of the system returning completely blank state.

Permanently delete a Doodle poll and all associated participant votes and comments
- **list_participants**: List all participants who voted on a Doodle poll
- **add_participant**: Provide a name and preference array (0=no, 1=yes, 2=if-need-be) matching option quantities.

Add a participant vote to a Doodle poll programmatically
- **remove_participant**: The core system inherently recalculates the total votes autonomously.

Remove a participant and their votes from a Doodle poll
- **get_comments**: Retrieve all comments on a Doodle poll
- **add_comment**: Add a comment to a Doodle poll
- **close_poll**: Overrides the core settings dictating finally which exact option value string won.

Close a Doodle poll and set the final chosen option


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Doodle** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my Doodle polls"

**🤖 AI Agent:**
> I found 3 polls in your account: 'Team Offsite Planning' (OPEN), 'Client Project Kickoff' (OPEN), and 'Monthly Sync' (CLOSED). Which one would you like to inspect for participant votes?

---

**👤 You:**
> "Create a poll 'Launch Sync' with options: 'Monday 10am', 'Tuesday 2pm'"

**🤖 AI Agent:**
> Poll created! 'Launch Sync' (ID: poll_abc123) is now active with 2 time options. You can now invite participants to vote on their preferred slots.

---

**👤 You:**
> "Who has voted on the 'Team Offsite' poll?"

**🤖 AI Agent:**
> Retrieving participants for 'Team Offsite'... 5 people have voted: 'Alice', 'Bob', 'Charlie', 'David', and 'Eve'. I can show you the detailed preference breakdown for each participant if you'd like.


## ❓ FAQ

**Q: Can my agent create a meeting poll with specific date and time options?**
Yes. Use the 'create_poll' tool. You can provide a JSON array of option strings (e.g., ['2026-04-01 10:00', '2026-04-02 14:00']). The agent will command the Doodle backend to generate the standard poll structure instantly.

**Q: How do I add a participant's vote programmatically via chat?**
Use the 'add_participant' tool. Provide the poll ID, the participant's name, and a JSON array of preference values (0=no, 1=yes, 2=if-need-be) matching the number of poll options. The agent will trigger the response routing instantly.

**Q: Can I close a poll and set the final meeting time through the agent?**
Absolutely. Use the 'close_poll' tool. Provide the poll ID and the text of the winning option. The agent will change the poll state to CLOSED, locking the participation arrays and officially confirming the chosen time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/doodle](https://vinkius.com/mcp/doodle)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Doodle** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `doodle` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Doodle** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "doodle": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
