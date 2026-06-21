# tl;dv MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tldv)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tldv-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tldv-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Record, transcribe, and clip key moments from Google Meet and Zoom calls so your team never misses important meeting insights.

## Description
Connect your **tl;dv** account to any AI agent and simplify how you manage your meeting recordings, transcripts, and AI-generated insights through natural conversation.

### What you can do

- **Meeting Oversight** — List all recorded meetings and retrieve detailed metadata, including participants and duration.
- **Transcript Access** — Fetch full transcriptions for any meeting to search for specific discussion points.
- **AI Insights** — Read AI-generated notes, summaries, and key moments (highlights) to quickly understand meeting outcomes.
- **External Import** — Programmatically import meeting recordings from external URLs for processing.
- **Content Retrieval** — Get direct download links for video recordings and access recent transcripts instantly.
- **Operational Monitoring** — Check API connectivity and account status directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your tl;dv API Key (found in your account settings)
3. Start managing your meeting knowledge base from Claude, Cursor, or any MCP client

### Who is this for?

- **Product Managers & Researchers** — quickly retrieve meeting summaries and highlights via simple AI queries.
- **Sales Teams** — verify discussion points and share transcripts directly from the workspace.
- **Operations Managers** — monitor meeting logs and maintain a central repository of recorded organizational knowledge via the AI assistant.


## Available Tools
- **get_api_status**: Check connection
- **get_recording_download**: Get video file URL
- **get_meeting_duration**: Check call length
- **get_meeting_highlights**: Get key moments
- **get_meeting_details**: Get meeting info
- **get_meeting_notes**: Read AI summaries
- **get_meeting_participants**: List attendees
- **get_meeting_transcript**: Read transcription
- **import_external_meeting**: Upload recording URL
- **list_recorded_meetings**: List recent meetings
- **list_recent_transcripts**: List latest transcripts
- **test_tldv_auth**: Verify credentials


## 💬 Prompt Examples

Here are some examples of how you can interact with the **tl;dv** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my recorded meetings from this month."

**🤖 AI Agent:**
> I've retrieved your meetings. You have 4 recent recordings including 'Q4 Roadmap Sync', 'User Interview - Alex', and 'Daily Standup'. Which one would you like the AI notes for?

---

**👤 You:**
> "Summarize the key decisions made in the 'Q4 Roadmap Sync' meeting."

**🤖 AI Agent:**
> Fetching AI notes... In the 'Q4 Roadmap Sync' (ID: mtg_10293), the team decided to prioritize the Mobile SDK, push the API redesign to Q1, and schedule a security audit for next week. Would you like the full highlight list?

---

**👤 You:**
> "Show me who attended the meeting with 'Alex' (ID: mtg_88231)."

**🤖 AI Agent:**
> I've retrieved the attendee list for mtg_88231. Participants included: Alex Rivera (External), Sarah Smith (Product), and Mike Ross (Engineering). The recording duration was 45 minutes.


## Installation & Usage

To install and use the **tl;dv** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tldv](https://vinkius.com/mcp/tldv)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
