# Granola MCP Server

Manage AI meeting notes via Granola — list and search meeting documents, retrieve transcripts and summaries, and track action items directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/granola)

## Overview
**Category:** productivity
**Tools Count:** 12

## Description
Connect your **Granola.ai** account to any AI agent and take full control of your AI-powered meeting notes, searchable conversation memory, and automated summaries through natural conversation.

### What you can do

- **Meeting Document Orchestration** — List all meeting documents in your workspace and retrieve primary entry points for workspace interactions natively
- **Live Content Retrieval** — Access full structured content of meeting documents, parsing human-modified annotations and ML-generated notes flawlessy
- **AI Summarization** — Retrieve synthesized AI-generated blocks reducing bulk meeting content into concise overviews and key takeaway nodes limitlessly
- **Action Item Tracking** — Isolate specifically categorized target steps inferred from recorded meeting intent to automate post-meeting follow-ups
- **Transcript Auditing** — Retrieve full speaker-detected transcripts parsed locally on device, containing semantic and chronological speech metadata natively
- **Participant Navigation** — Identify meeting attendees by cross-referencing calendar arrays bound to Granola sessions synchronously
- **Global Workspace Search** — Execute full-text term detection across all documents to find specific discussions and prioritized ranked datasets
- **Folder & List Management** — Enumerate high-level categorization labels grouping documents physically inside directories to browse your workspace hierarchy
- **Batch Retrieval Oversight** — Fetch multiple meeting documents by their IDs in a single request to analyze complex cross-meeting dependencies securely

### How it works

1. Subscribe to this server
2. Enter your Granola API Key (found in your Granola Settings)
3. Start managing your meeting notes and searchable memory from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Managers & Team Leads** — summarize back-to-back meetings and track action items without manual note-taking
- **Product Managers** — audit collaborative meeting documents and search across conversation history using natural language
- **Executive Assistants** — organize meeting folders and retrieve participant metadata through the chat interface
- **Operations Teams** — monitor organizational knowledge and verify meeting results in real-time through natural conversation


## Available Tools
- **list_documents**: List all meeting documents in the Granola workspace with pagination
- **get_metadata**: Retrieve metadata for a specific meeting document
- **get_transcript**: Retrieve the full transcript of a meeting with speaker detection
- **get_documents_batch**: Fetch multiple documents by their IDs in a single request
- **list_folders**: List all document lists (folders) in the Granola workspace
- **get_content**: Retrieve the full structured content of a meeting document
- **list_by_date**: List meeting documents within a specific date range
- **get_participants**: Retrieve the list of participants for a specific meeting
- **get_summary**: Retrieve the AI-generated summary of a meeting document
- **list_recent**: List the 20 most recent meeting documents
- **get_action_items**: Extract action items identified from a meeting document
- **search_documents**: Full-text search across all meeting documents


## Installation & Usage

To install and use the **Granola** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/granola](https://vinkius.com/mcp/granola)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
