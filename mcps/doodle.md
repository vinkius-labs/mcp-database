# Doodle MCP Server

Manage group scheduling via Doodle — create meeting polls, track participant votes, handle comments, and close polls directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/doodle)

## Overview
**Category:** productivity
**Tools Count:** 10

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


## Available Tools
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


## Installation & Usage

To install and use the **Doodle** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/doodle](https://vinkius.com/mcp/doodle)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
