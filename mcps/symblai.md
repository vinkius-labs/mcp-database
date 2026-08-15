# Symbl.ai MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/symblai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Extract conversation intelligence from audio, video, and text — get summaries, action items, and topics directly from any AI agent.

## Description
Connect **Symbl.ai** to your AI agent to unlock deep insights from your meetings, calls, and chats. Transform raw audio, video, or text into structured intelligence through natural conversation.

### What you can do

- **Media Intelligence** — Process audio and video files (base64) or text payloads to generate unique conversation IDs for analysis.
- **Automated Summarization** — Generate concise summaries of long conversations to capture the essence without manual review.
- **Actionable Insights** — Extract action items, follow-ups, and questions automatically to keep your team and projects moving.
- **Topic Discovery** — Identify the main themes and topics discussed across your communication channels.
- **Custom Trackers** — Create trackers for specific keywords or phrases to monitor compliance, sentiment, or specific interests.

### How it works

1. Subscribe to this server
2. Enter your Symbl.ai App ID and App Secret
3. Start analyzing your conversations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — Quickly digest user interviews and stakeholder meetings to find key requirements.
- **Sales Teams** — Identify follow-up opportunities and customer pain points from call transcripts instantly.
- **Developers** — Integrate conversation intelligence into your workflow without building complex NLP pipelines.


## Available Tools (9)
- **create_tracker**: Create a tracker to detect specific keywords or phrases
- **get_action_items**: Get action items from a processed conversation
- **get_follow_ups**: Get follow-ups from a processed conversation
- **get_questions**: Get questions from a processed conversation
- **get_summary**: Get summary of a processed conversation
- **get_topics**: Get topics from a processed conversation
- **process_audio**: ai for processing. Returns a conversation ID.

Process an audio file to extract insights
- **process_text**: ai. Returns a conversation ID.

Process text conversations to extract insights
- **process_video**: ai for processing. Returns a conversation ID.

Process a video file to extract insights


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Symbl.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract action items from conversation ID '549201834752'."

**🤖 AI Agent:**
> I've analyzed the conversation. Here are the action items: 1. John to update the API docs by Friday. 2. Sarah to schedule a follow-up with the client.

---

**👤 You:**
> "Summarize the meeting with ID '982374102'."

**🤖 AI Agent:**
> The meeting focused on the Q3 roadmap. Key points included the launch of the new dashboard and the migration to the new cloud provider.

---

**👤 You:**
> "What were the main topics discussed in conversation 'abc-123'?"

**🤖 AI Agent:**
> The main topics identified are: 'Budget Allocation' (relevance: 0.95), 'Hiring Plan' (relevance: 0.88), and 'Office Reopening' (relevance: 0.72).


## ❓ FAQ

**Q: How do I get a summary of a processed conversation?**
Use the `get_summary` tool by providing the specific Conversation ID. The agent will return a structured summary of the key points discussed.

**Q: Can I detect specific keywords in my audio or text files?**
Yes! Use the `create_tracker` tool to define a list of keywords or phrases. Symbl.ai will then monitor and detect these within your processed conversations.

**Q: What insights can I extract from a conversation ID?**
You can use `get_topics`, `get_action_items`, `get_follow_ups`, and `get_questions` to retrieve specific intelligence layers from any previously processed media.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/symblai](https://vinkius.com/mcp/symblai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Symbl.ai** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `symblai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Symbl.ai** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "symblai": {
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
