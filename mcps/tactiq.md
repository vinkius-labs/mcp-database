# Tactiq MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tactiq)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage meeting transcripts via Tactiq u2014 access summaries, action items, speaker analytics, and search across all recordings from your AI agent.

## Description
Connect your **Tactiq** account to any AI agent and manage all your meeting transcripts, summaries, and follow-ups through natural conversation.

### What you can do

- **Transcript Management** u2014 List, search, and retrieve full meeting transcripts with speaker labels and timestamps
- **Meeting Intelligence** u2014 Access AI-generated summaries, insights, and key decisions from every recorded meeting
- **Action Items** u2014 Extract follow-ups, deadlines, and assigned tasks automatically from any transcript
- **Speaker Analysis** u2014 View speaker participation, talk-time ratios, and contribution breakdowns
- **Cross-Meeting Search** u2014 Search across your entire transcript library for any keyword, topic, or discussion point

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Tactiq dashboard (Settings > Integrations)
3. Start managing your meeting knowledge from Claude, Cursor, or any MCP client

No more manual searching for 'who said what' or missing critical meeting follow-ups. Your AI agent becomes your dedicated meeting assistant.

### Who is this for?

- **Project Managers** u2014 retrieve meeting summaries and track action items instantly
- **Product Leads** u2014 review transcript details and decision history without context-switching
- **Developers** u2014 integrate Tactiq transcript data into custom workflows via simple AI queries


## Available Tools (6)
- **list_meetings**: Available on all Tactiq plans (Free, Pro, Team).

List recent meetings
- **list_meeting_artifacts**: Requires Tactiq Team plan or higher.

List AI artifacts from a meeting
- **check_generation_status**: Useful when a summary is still being processed by Tactiq AI. Returns the current processing state.

Check if meeting summary is ready
- **get_artifact**: Artifacts include action items, email drafts, slide outlines, and more.

Read a specific AI artifact
- **get_meeting_summary**: Requires Tactiq Team plan or higher. Returns key takeaways, decisions, and context.

Get AI-generated meeting summary
- **search_meetings**: Use to find specific discussions: "Find my calls with the design team from last month" or "What was decided about Q1 roadmap?"

Search meetings by keyword, participant, or date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tactiq** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all meetings from this week."

**🤖 AI Agent:**
> You had 8 meetings this week. The longest was 'Q2 Planning' (62 min, 5 participants). Would you like to see the summary or action items from any meeting?

---

**👤 You:**
> "Get the summary and action items from transcript TR-5021."

**🤖 AI Agent:**
> Summary: The team agreed on Q2 priorities, assigned 3 tasks (proposal draft by Friday, budget review next Monday, client follow-up by Sarah). 4 key decisions were made. Want me to format these as tasks?

---

**👤 You:**
> "Search my transcripts for mentions of 'pricing strategy'."

**🤖 AI Agent:**
> Found 5 mentions across 3 meetings. The most detailed discussion was in 'Sales Review' (March 18), where the team spent 12 minutes on pricing tiers. Would you like to read that section?


## ❓ FAQ

**Q: How do I access meeting transcripts via AI?**
Use `list_transcripts` to see all recorded meetings, then `get_transcript` with the transcript ID for the full text with speaker labels and timestamps.

**Q: Can I extract action items from meetings?**
Yes. Use `get_action_items` with a transcript ID to retrieve all AI-detected follow-ups, deadlines, and assigned tasks.

**Q: How do I search across all my transcripts?**
Use `search_transcripts` with any keyword or phrase to find matching content across all recorded meetings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tactiq](https://vinkius.com/mcp/tactiq)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tactiq** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tactiq` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tactiq** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tactiq": {
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
