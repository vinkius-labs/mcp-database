# National Archives Catalog MCP Server

Search and explore millions of historical documents, photos, and records from the US National Archives (NARA) directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/national-archives-catalog)

## Overview
**Category:** knowledge-management
**Tools Count:** 40

## Description
Connect to the **National Archives Catalog (NARA)** and explore the history of the United States through natural conversation. This MCP server allows your AI agent to act as a specialized research assistant, retrieving historical data, metadata, and digital objects from one of the world's largest archival collections.

### What you can do

- **Deep Search** — Query records by text, tags, comments, or transcriptions to find specific historical context and documents.
- **Record Hierarchy** — Navigate complex archival structures by retrieving immediate children of specific parent records (NaId).
- **User Contributions** — Manage and search through tags, comments, and transcriptions provided by the citizen archivist community.
- **Metadata Retrieval** — Get detailed information, status metrics, and descriptions for specific National Archives Identifiers.
- **Tagging & Interaction** — Create or delete tags and comments to organize research findings directly within the catalog ecosystem.

### How it works

1. Subscribe to this server
2. Enter your NARA API Key
3. Start researching history from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Historians & Researchers** — instantly retrieve primary source documents and metadata without manual catalog navigation.
- **Educators** — find relevant historical photos and records to build curriculum materials directly from a chat interface.
- **Genealogists** — search through millions of records and transcriptions to find family history data and archival links.


## Available Tools
- **create_comment**: Add a new comment to a record
- **create_tag**: Add a new tag to a record
- **create_transcription**: Add a new transcription
- **delete_comment**: Remove or deactivate a comment
- **delete_contributions**: Deactivate or remove multiple contributions
- **delete_tag**: Remove or deactivate a tag
- **fetch_coords**: Utility to fetch JSON data from S3 based on a provided URL
- **get_announcements**: Retrieve a list of all announcements
- **get_comment**: Retrieve a single comment by ID
- **get_comments_by_naid**: Retrieve comments for a specific record
- **get_comments_by_userid**: Retrieve comments by a specific contributor
- **get_contributions_by_target_naid**: Retrieve contributions for a specific record ID
- **get_contributions_by_userid**: Retrieve contributions by user ID
- **get_justifications**: Retrieve a list of justifications for administrative actions
- **get_latest_announcements**: Retrieve active announcements
- **get_record_children**: Retrieve immediate children of a specified parent ID
- **get_record_stats**: Retrieve statistics on user contributions
- **get_tag**: Retrieve a single tag by ID
- **get_tags_by_naid**: Retrieve tags for a specific record
- **get_tags_by_userid**: Retrieve tags by a specific contributor
- **get_transcription_history**: Retrieve transcription history
- **get_transcription**: Retrieve a single transcription by ID
- **get_transcriptions_by_naid**: Retrieve transcriptions for a specific record
- **get_transcriptions_by_userid**: Retrieve transcriptions by a specific contributor
- **get_user_notifications**: Retrieve user notifications
- **get_user**: Retrieve public data for a specific user
- **get_users**: Retrieve public account data (filterable by email, username, role, etc.)
- **search_comments**: Search for comment data
- **search_contributions**: Search for contribution data
- **search_records_by_comment**: Search records by comments
- **search_records_by_contribution**: Search records related to user contributions
- **search_records_by_tag**: Search records by tags
- **search_records_by_text**: Search records by other extracted text
- **search_records_by_transcription**: Search records by transcriptions
- **search_records**: Search for records using URL parameters
- **search_tags**: Search for tag data
- **search_transcriptions**: Search for transcription data
- **update_comment**: Update an existing comment
- **update_transcription**: Add or update a transcription
- **update_user**: Update user information


## Installation & Usage

To install and use the **National Archives Catalog** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/national-archives-catalog](https://vinkius.com/mcp/national-archives-catalog)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
