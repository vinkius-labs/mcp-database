# Quip MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/quip)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Connect Quip to your AI to search documents, read threads, view messages, and edit content seamlessly.

## Description
Integrate your **Quip** (Salesforce) account with any AI agent to bring your real-time collaborative documents, spreadsheets, and team discussions directly into your workflow.

### What you can do

- **Document Search** — Perform full-text searches across all your accessible Quip documents, or fetch recently accessed threads to resume your work.
- **Read & Retrieve** — Navigate the folder hierarchy and retrieve full content, extracting documentation, plans, and metadata without leaving your IDE.
- **Review Conversations** — Check document-attached messages to stay up-to-date on feedback and team discussions.
- **Edit & Append** — Programmatically update documents by passing HTML payloads back to specific Quip threads.

### How it works

1. Subscribe to this server.
2. Authorize using a Quip Personal Access Token.
3. Instruct your AI to fetch specifications or draft content directly into Quip.

### Who is this for?

- **Developers** — Fetch technical specifications or PRD texts directly from a Quip link before writing code.
- **Product Managers** — Summarize recent comments on product strategy documents.
- **Account Executives** — Draft client updates and push the finalized HTML text into a shared Quip document.


## Available Tools
- **get_current_user**: Retrieves the authenticated user profile
- **get_thread**: Retrieves a single Quip document or thread by ID
- **get_threads**: Provide a comma-separated list of IDs.

Batch-fetches multiple Quip threads by their IDs
- **get_recent_threads**: Retrieves recently viewed or edited documents
- **search_threads**: Performs a full-text search across accessible Quip documents
- **get_folder**: Retrieves details for a specific Quip folder
- **get_folders**: Provide a comma-separated list of IDs.

Batch-fetches multiple Quip folders by their IDs
- **get_messages**: Lists chat messages or comments attached to a thread
- **get_user**: Retrieves profile information for a specific user
- **get_contacts**: Lists all collaborators of the authenticated user
- **list_blobs**: Lists embedded files and images in a thread
- **edit_document**: You must provide HTML content.

Edits content in a Quip document


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Quip** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search Quip for documents containing 'Q3 Roadmap'."

**🤖 AI Agent:**
> I ran `search_threads` for 'Q3 Roadmap' and found 2 relevant documents:
1. 'Engineering Q3 Roadmap' (ID: ABC123DEF)
2. 'Design Team Syncs - Q3 Roadmap' (ID: XYZ987JKL)
Would you like me to retrieve the contents of the Engineering thread?

---

**👤 You:**
> "What documents did I work on recently in Quip?"

**🤖 AI Agent:**
> Using `get_recent_threads`, here are your latest documents:
- 'Sprint 44 Retrospective' - Modified today.
- 'Marketing Copy Ideas' - Modified yesterday.
- 'Q3 Budget Tables' - Modified on Tuesday.

---

**👤 You:**
> "Add a new heading called 'Conclusion' and a paragraph 'All tests passed' to document ABC123DEF."

**🤖 AI Agent:**
> I successfully edited the thread 'ABC123DEF' using the HTML payload: `<h2>Conclusion</h2><p>All tests passed</p>`. The content has been added to the document.


## ❓ FAQ

**Q: How do I securely obtain my Quip Access Token?**
Sign in to your Quip account. Navigate to your API token generator page (usually at `platform.quip.com` or via Quip's Developer Settings). Generate a **Personal Access Token**, copy the string, and securely save it in the configuration fields below.

**Q: Can I provide a Quip document URL to my AI, or just the ID?**
You can provide the standard URL. The agent is capable of recognizing the URL structure, extracting the alphanumeric `thread_id`, and performing the operation accurately.

**Q: Can it read embedded images or files inside the document?**
The agent detects their existence by reading the raw structure and uses `list_blobs` to catalog attachments. However, downloading the actual files depends on your client's supported capabilities.

**Q: Is the edit operation destructive?**
The `edit_document` function uses Quip's native append logic to add new HTML blocks at the end of the document, mitigating complete overwrites. Additionally, Quip maintains a full version history allowing rollbacks if necessary.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/quip](https://vinkius.com/mcp/quip)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Quip** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `quip` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Quip** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "quip": {
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
