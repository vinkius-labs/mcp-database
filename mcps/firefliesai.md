# Fireflies.ai MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/firefliesai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/firefliesai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/firefliesai-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transcribe meetings, analyze conversation metrics, and query transcripts via AI agents with Fireflies.ai.

## Description
Connect your **Fireflies.ai** account to any AI agent and unlock the power of meeting intelligence through the Model Context Protocol (MCP). Fireflies.ai automates your meeting notes, transcribes conversations across several platforms, and provides deep analytics to help your team stay aligned. Now, you can query your entire meeting history and manage your transcription bot directly through natural conversation.

### What you can do

- **Transcript Retrieval** — List recent meetings and fetch detailed summaries, action items, and keywords from any transcript.
- **AskFred Integration** — Leverage Fireflies' AI assistant (AskFred) to ask questions about your meetings or start new analysis threads.
- **Live Bot Control** — Invite the Fireflies bot to ongoing meetings (Zoom, Google Meet, etc.) by simply providing the meeting URL.
- **Conversation Analytics** — Access aggregate metrics like talk-to-listen ratios and words-per-minute to improve team communication.
- **User & Team Management** — List team members and fetch user-specific meeting metadata.
- **Transcript Management** — Rename transcripts or delete them to keep your meeting database organized and up to date.
- **Real-time Monitoring** — See which meetings are currently being recorded and transcribed in real-time.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Fireflies API Key (found in your Integrations > Fireflies API settings)
3. Start managing your meeting intelligence from Claude, Cursor, or any MCP client

### Who is this for?

- **Project Managers** — quickly pull action items and summaries from recent project syncs without re-watching recordings.
- **Sales Teams** — analyze talk-to-listen ratios and sentiment across discovery calls to refine your sales pitch.
- **Executive Assistants** — automate the organization and renaming of meeting transcripts through simple AI commands.


## Available Tools
- **add_to_live_meeting**: Invite Fireflies to a live meeting
- **create_ask_fred_thread**: Ask a question to AskFred
- **delete_transcript**: Delete a transcript
- **get_analytics**: Get meeting analytics
- **get_ask_fred_thread**: Get AskFred thread messages
- **get_transcript**: Get transcript details
- **get_user**: Get user details
- **list_active_meetings**: List meetings currently being recorded
- **list_ask_fred_threads**: List AskFred threads
- **list_transcripts**: List recent transcripts
- **list_users**: List team users
- **update_meeting_title**: Rename a meeting


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fireflies.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my 5 most recent meeting transcripts."

**🤖 AI Agent:**
> Fetching transcripts... I found 5 recent meetings, including 'Product Roadmap Sync' and 'Q1 Review'. Would you like the AI summary or action items for any of these?

---

**👤 You:**
> "Invite Fireflies to join my current meeting at https://zoom.us/j/123456789"

**🤖 AI Agent:**
> Request sent! I've invited the Fireflies bot to your Zoom meeting. It should join shortly to start transcribing the conversation.

---

**👤 You:**
> "Show me the action items from meeting ID 'trans_987'."

**🤖 AI Agent:**
> Retrieving summary... For meeting 'trans_987', the action items are: 1) Update the landing page design, 2) Send the final proposal by Friday, and 3) Schedule a follow-up call with the engineering team.


## Installation & Usage

To install and use the **Fireflies.ai** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/firefliesai](https://vinkius.com/mcp/firefliesai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
