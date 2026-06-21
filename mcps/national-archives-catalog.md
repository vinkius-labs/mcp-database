# National Archives Catalog MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/national-archives-catalog)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Search and explore millions of historical documents, photos, and records from the US National Archives (NARA) directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **National Archives Catalog** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for records related to the 'Apollo 11 mission'."

**🤖 AI Agent:**
> I've found several records. The most prominent is the 'Apollo 11 Flight Plan' (NaId: 594912). Would you like to see its metadata or check for related children records?

---

**👤 You:**
> "Get the immediate children of parent record 573036."

**🤖 AI Agent:**
> Retrieving children for NaId 573036... I found several items including 'Logbook of the USS Constitution' and 'Correspondence files'. Which one should I inspect further?

---

**👤 You:**
> "Find all tags associated with record NaId 123456."

**🤖 AI Agent:**
> I've retrieved the tags for NaId 123456. Current tags include: 'World War II', 'Naval Intelligence', and 'Pacific Theater'. Would you like to add a new tag to this record?


## ❓ FAQ

**Q: Can I search for records specifically by the text in their transcriptions?**
Yes. Use the `search_records_by_transcription` tool. This is particularly useful for handwritten documents that have been digitized and transcribed by volunteers.

**Q: How do I see the individual items within a larger archival series?**
Use the `get_record_children` tool with the parent `NaId`. This will list the immediate sub-records or files contained within that specific collection or series.

**Q: Can I contribute to the archives by adding tags via the AI?**
Yes, the `create_tag` tool allows you to add descriptive tags to a record using its National Archives Identifier (NaId), helping improve searchability for the community.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/national-archives-catalog](https://vinkius.com/mcp/national-archives-catalog)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **National Archives Catalog** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `national-archives-catalog` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **National Archives Catalog** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "national-archives-catalog": {
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
