# Fathom MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fathom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage AI meeting notes via Fathom — list and search meetings, retrieve transcripts and summaries, and track action items directly from any AI agent.

## Description
Connect your **Fathom.video** account to any AI agent and take full control of your meeting intelligence and automated note-taking through natural conversation.

### What you can do

- **Meeting Orchestration** — List recent meetings and search across your entire recording history to retrieve titles, dates, and participant metadata natively
- **AI Transcription** — Retrieve full speaker-attributed transcripts with timestamps to review exact discussions and verbal commitments limitlessly
- **Contextual Summarization** — Get AI-generated summaries distilling key discussion points, decisions, and overall meeting context into a concise format
- **Action Item Tracking** — Extract AI-identified tasks with assigned owners and due dates to automate post-meeting follow-up workflows
- **Recording Management** — Access video and audio recording URLs for immediate streaming or download bypassing the web interface
- **Attendee Auditing** — List all meeting participants including join/leave times and speaking duration to verify engagement levels synchronously
- **Team Intelligence** — Access meetings shared with your Fathom team to monitor cross-functional discussions and organizational knowledge securely
- **Highlight Navigation** — Retrieve specific moments flagged as important during calls to focus on critical insights without reviewing entire recordings

### How it works

1. Subscribe to this server
2. Enter your Fathom API Key (found in Fathom Settings > Integrations > API)
3. Start managing your meeting intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers & Leads** — summarize team syncs and track action items without manual note-taking
- **Sales & Success Teams** — quickly look up customer call transcripts and verify verbal commitments using natural language
- **Researchers** — search across multiple interview recordings and extract key highlights directly from the chat
- **Operations Teams** — monitor team meeting attendance and audit shared knowledge through natural conversation


## Available Tools (12)
- **get_action_items**: Get AI-identified action items for a meeting
- **get_attendees**: Get the list of participants for a meeting
- **get_highlights**: Get important moments flagged in a meeting
- **get_me**: Get current API token user profile
- **get_meeting**: Get details for a specific Fathom meeting
- **get_recording**: Get the recording URLs for a meeting
- **get_summary**: Get the AI-generated summary for a meeting
- **get_team_meetings**: List meetings shared with your team
- **get_transcript**: Get the full transcript for a meeting
- **get_webhooks**: List configured webhooks
- **list_meetings**: List all Fathom meetings
- **search_meetings**: Search for meetings by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fathom** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the summary and action items for my last meeting"

**🤖 AI Agent:**
> Retrieving your last meeting... Title: 'Project Alpha Kickoff'. Summary: The team aligned on the Q2 roadmap and budget. Action Items: 1. John to send draft spec by Friday. 2. Sarah to schedule follow-up with stakeholders.

---

**👤 You:**
> "Search my meetings for mentions of 'pricing strategy'"

**🤖 AI Agent:**
> Searching meetings... I found 2 recordings mentioning 'pricing strategy': 'Monthly Business Review' (March 15) and 'Pricing Workshop' (Feb 20). Would you like the transcript snippets for these mentions?

---

**👤 You:**
> "Get the transcript for meeting 'abc-123'"

**🤖 AI Agent:**
> Retrieving transcript... I have the full speaker-attributed text for 'Product Roadmap Sync'. [Agent displays snippet of transcript]. Would you like me to export this or search for specific details within it?


## ❓ FAQ

**Q: Can my agent retrieve the summary of a specific meeting from Fathom?**
Yes. Use the 'get_summary' tool. Provide the meeting ID, and the agent will return the AI-distilled context, including key discussion points and decisions made during the call natively.

**Q: How do I extract action items from a call via chat?**
Use the 'get_action_items' tool. Your agent will parse the AI-identified tasks, returning assigned owners and descriptions, making it easy to automate your follow-up workflows.

**Q: Can I search for meetings where a specific keyword was mentioned through the agent?**
Absolutely. Use the 'search_meetings' tool. Provide your query, and the agent will search through titles, transcripts, and summaries to find matching meetings across your entire Fathom history.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fathom](https://vinkius.com/mcp/fathom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fathom** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fathom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fathom** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fathom": {
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
