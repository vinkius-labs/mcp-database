# Fireflies.ai MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/firefliesai-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Record, transcribe, and search across all your meetings with AI that captures every conversation and makes it instantly findable.

## Description
Connect your **Fireflies.ai** account to any AI agent and take full control of your meeting documentation and conversational knowledge retrieval through natural conversation.

### What you can do

- **Meeting Orchestration** — List and manage meeting transcripts programmatically, including retrieving AI summaries, action items, and complete text logs
- **Live Transcription** — Programmatically invite the Fireflies bot to ongoing Zoom, Google Meet, or Teams calls for real-time recording and documentation
- **Transcript Intelligence** — Use 'AskFred' to ask complex natural language questions about specific meeting contents and retrieve instant, high-fidelity answers
- **Asset Management** — Upload public audio URLs for automated transcription and manage meeting soundbites to preserve critical conversation clips
- **Organizational Visibility** — Retrieve team member directories and account metadata to coordinate meeting knowledge across your entire workspace

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Fireflies.ai settings (Settings > API)
3. Start managing your meeting intelligence from Claude, Cursor, or any MCP client

No more manual note-taking or scrubbing through hours of recordings to find a decision. Your AI acts as your dedicated meeting analyst and knowledge coordinator.

### Who is this for?

- **Product Managers** — instantly retrieve action items and summaries from user research calls using natural language
- **Sales Teams** — monitor customer sentiment and identify key pain points from recent demos without leaving your workspace
- **Operations Leads** — automate the documentation of team syncs and manage meeting access across the organization


## Available Tools
- **add_to_live_meeting**: Invite bot to live call
- **ask_fred**: Ask AI about a meeting
- **delete_transcript**: Delete a meeting record
- **get_account_info**: Get my profile
- **get_ai_app_outputs**: Get AI App responses
- **get_transcript**: Get transcript details
- **list_soundbites**: List meeting soundbites
- **list_transcripts**: List all meeting transcripts
- **list_team_users**: List organization users
- **list_webhooks**: List active webhooks
- **update_meeting_title**: Update meeting title
- **upload_audio**: Transcribe audio file


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fireflies.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Summarize the key decisions from the meeting 'Project Alpha Sync'."

**🤖 AI Agent:**
> Retrieving summary... I've identified 3 key decisions from Project Alpha Sync: 1. Launch is delayed to Q4. 2. Budget is increased by 10%. 3. John is lead on API docs. Would you like the full action items list?

---

**👤 You:**
> "Invite the Fireflies bot to this Meet link: [url]."

**🤖 AI Agent:**
> Done! I've sent the invitation to your live meeting. The Fireflies bot will join shortly to begin recording and transcribing the conversation.

---

**👤 You:**
> "Ask Fred: 'What was the specific feedback regarding the mobile UI?' for meeting '123'."

**🤖 AI Agent:**
> AskFred analysis... According to the transcript, the client mentioned that the navigation buttons are too small for smaller devices and the color contrast needs to be improved. Should I create a task for the design team?


## ❓ FAQ

**Q: How do I find my Fireflies API Key?**
Log in to your Fireflies.ai dashboard, navigate to **Settings** > **API**, and copy your unique token.

**Q: What is AskFred?**
AskFred is an AI-powered meeting assistant that can answer questions about any of your recorded meetings based on their transcript data.

**Q: Can I record a meeting that is already in progress?**
Yes! Use the `add_to_live_meeting` tool and provide the join URL. The Fireflies bot will attempt to join the call immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/firefliesai-alternative](https://vinkius.com/mcp/firefliesai-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fireflies.ai** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `firefliesai-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fireflies.ai** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "firefliesai-alternative": {
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
