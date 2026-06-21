# Fellow MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fellow)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fellow-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fellow-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-operations](../categories/business-operations.md)

Manage meeting notes and feedback via Fellow — list agenda items and decisions, track action items, handle recordings, and complete tasks directly from any AI agent.

## Description
Connect your **Fellow.app** account to any AI agent and take full control of your meeting management, collaborative agendas, and action item tracking through natural conversation.

### What you can do

- **Meeting Note Orchestration** — List all meeting notes and retrieve full structured content including agenda items, discussion points, and decision metadata natively
- **Action Item Auditing** — List and filter all tasks across meetings to track descriptions, assignees, and due dates for cross-meeting accountability flawlessly
- **Recording Management** — Browse meeting recordings and retrieve video/audio details including time-limited download or stream URLs securely
- **AI Transcription Retrieval** — Fetch full transcripts with speaker attribution and timestamps to review critical discussions or extract specific insights limitlessly
- **Task Lifecycle Control** — Mark action items as complete or archive them to manage your active workspace and notify relevant stakeholders synchronously
- **Identity Oversight** — Retrieve the authenticated profile identity including name, email, and workspace contexts to verify permission limits natively
- **Data Invalidation** — Irreversibly vaporize specific meeting notes or recordings findable by ID to manage your organizational records strictly

### How it works

1. Subscribe to this server
2. Enter your Fellow API Key (found in User Settings > Account > API Tokens)
3. Start managing your meeting notes and tasks from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Managers & Team Leads** — track team action items and review meeting decisions without manual follow-ups
- **Product Managers** — audit collaborative agendas and search across meeting transcripts using natural language
- **Executive Assistants** — manage meeting recordings and organize documentation for stakeholders through the chat interface
- **Operations Teams** — verify cross-meeting task statuses and monitor organizational knowledge in real-time


## Available Tools
- **list_notes**: Use as the primary entry point to browse all meeting documentation.

List all meeting notes in the Fellow workspace
- **get_note**: Essential for reviewing a specific meeting.

Retrieve the full content and metadata of a specific meeting note by ID
- **delete_note**: Confirm with the user before executing — this cannot be undone.

Permanently delete a meeting note by ID
- **list_recordings**: Use to browse all recorded meetings.

List all meeting recordings captured by Fellow
- **get_recording**: Use to access a specific recording.

Retrieve details of a specific meeting recording
- **delete_recording**: Confirm with the user before executing.

Permanently delete a meeting recording by ID
- **get_transcript**: Use for detailed review, compliance documentation, or extracting specific discussion points.

Retrieve the full transcript of a meeting recording
- **list_action_items**: Use for cross-meeting task tracking and accountability.

List all action items across all meetings
- **get_action_item**: Use to inspect a single task.

Retrieve details of a specific action item by ID
- **complete_action_item**: Use when a task has been finished.

Mark an action item as complete
- **archive_action_item**: Archive an action item, removing it from active views without deleting it
- **get_current_user**: Use to verify which account is connected.

Retrieve the authenticated Fellow user profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fellow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all my pending action items"

**🤖 AI Agent:**
> Retrieving action items... I found 5 pending tasks. Highlights include 'Update Q2 Roadmap' (Due Tomorrow) and 'Send follow-up to Client A'. Would you like the ID for any of these to mark them as complete?

---

**👤 You:**
> "Get the notes for the meeting 'Product Sync' from last Tuesday"

**🤖 AI Agent:**
> Found it! The notes for 'Product Sync' (March 24) include 3 agenda items and 2 finalized decisions regarding the feature launch. I can display the full discussion points for you.

---

**👤 You:**
> "List the last 3 meeting recordings"

**🤖 AI Agent:**
> Retrieving recordings... Here are the 3 most recent: 'Strategic Planning' (1h 20m), 'Daily Standup' (15m), and 'Design Review' (45m). Which one would you like the transcript or recording URL for?


## Installation & Usage

To install and use the **Fellow** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fellow](https://vinkius.com/mcp/fellow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
