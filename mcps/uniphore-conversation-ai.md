# Uniphore Conversation AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uniphore-conversation-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Access meeting transcripts, summaries, action items, and analytics via Uniphore API.

## Description
Connect **Uniphore** to any AI agent and unlock powerful conversation intelligence -- retrieve meeting transcripts, AI-generated summaries, action items, and analytics through natural conversation.

### What you can do
- **Meeting Transcripts** -- Get speaker-tagged transcripts of any recorded call or meeting
- **AI Summaries** -- Retrieve concise summaries of key discussion points
- **Action Items** -- Extract next steps and tasks identified during meetings
- **Conversation Analytics** -- View talk ratios, sentiment, topics, and engagement metrics
- **Search Meetings** -- Find past meetings by keyword or topic discussed

### How it works
1. Subscribe to this server
2. Enter your Uniphore Access Token and Organization ID
3. Start analyzing conversations from Claude, Cursor, or any MCP-compatible client

Uniphore is a leading Conversation AI platform used by sales, support, and success teams to automate meeting notes, track customer sentiment, and uncover revenue insights.

### Who is this for?
- **Sales Teams** -- Review call transcripts and action items to follow up on opportunities
- **Support Managers** -- Monitor conversation analytics and customer sentiment
- **Operations** -- Search past meetings for specific topics or compliance keywords


## Available Tools (8)
- **get_action_items**: Get action items extracted from a meeting
- **get_meeting_analytics**: Get conversation analytics and insights for a meeting
- **get_meeting**: Get details of a specific meeting
- **list_meetings**: Use this to discover meeting IDs before querying specific details.

List all recorded meetings and calls
- **search_meetings**: Search meetings by keyword or topic
- **get_meeting_summary**: Get the AI-generated summary of a meeting
- **list_topics**: List all tracked topics and keywords in the organization
- **get_transcript**: Get the full transcript of a meeting


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Uniphore Conversation AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the summary for meeting MTG-123."

**🤖 AI Agent:**
> Meeting Summary: Discussed Q4 targets, agreed on new pricing strategy, and scheduled follow-up for next week.

---

**👤 You:**
> "Get the transcript for meeting MTG-456."

**🤖 AI Agent:**
> Transcript:
- Agent: Thanks for joining. What can I help with today?
- Customer: I have a question about my recent invoice.

---

**👤 You:**
> "What are the action items from the last sales call?"

**🤖 AI Agent:**
> Action Items:
1. Send pricing proposal to client (Assignee: John Doe)
2. Schedule technical demo for next Tuesday (Assignee: Jane Smith)


## ❓ FAQ

**Q: How do I get my Uniphore Access Token and Org ID?**
Log in to your Uniphore account, navigate to Settings > API Access, and generate a new token. Your Organization ID is displayed in the same settings panel.

**Q: Can I get AI-generated summaries of meetings?**
Yes! Use the get_meeting_summary tool with a meeting ID to retrieve the concise AI summary of that call.

**Q: Can I extract action items from a call?**
Yes! Use the get_action_items tool with a meeting ID. Uniphore AI identifies next steps and assigns them to speakers if possible.

**Q: Can I search for specific topics in past meetings?**
Yes! Use the search_meetings tool with relevant keywords or topic names to find matching recorded calls.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uniphore-conversation-ai](https://vinkius.com/mcp/uniphore-conversation-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Uniphore Conversation AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `uniphore-conversation-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Uniphore Conversation AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "uniphore-conversation-ai": {
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
