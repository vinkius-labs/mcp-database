# Granola MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/granola)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage AI meeting notes via Granola — list and search meeting documents, retrieve transcripts and summaries, and track action items directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Granola** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the 5 most recent meeting documents"

**🤖 AI Agent:**
> Retrieving your recent documents... I found 5 meetings including 'Product Design Workshop', 'Q2 Budget Review', and 'Weekly Sync'. Would you like the AI summary or the list of participants for the design workshop?

---

**👤 You:**
> "What were the action items from meeting 'abc-123'?"

**🤖 AI Agent:**
> Action items extracted! For meeting abc-123, I found 3 tasks: 1. John to update the landing page copy. 2. Sarah to finalize the pricing model. 3. Mike to schedule the stakeholder demo. Would you like the due dates for these?

---

**👤 You:**
> "Search for meeting notes mentioning 'competitor analysis'"

**🤖 AI Agent:**
> Searching documents... I found 2 meeting documents mentioning 'competitor analysis'. The most relevant is 'Marketing Strategy Sync' from March 20. I can retrieve the full structured content or transcript for you.


## ❓ FAQ

**Q: Can my agent retrieve the AI summary of a specific Granola meeting?**
Yes. Use the 'get_summary' tool. The agent will fetch the native generative results, reducing the bulk meeting content into synthesized blocks and key takeaways flawlessly.

**Q: How do I extract action items from recorded notes via chat?**
Use the 'get_action_items' tool. Your agent will isolate targeted steps inferred from the meeting intent, enabling you to automate your post-meeting follow-up workflows natively.

**Q: Can I search for meetings from a specific date range through the agent?**
Absolutely. Use the 'list_by_date' tool. Provide the start and end dates in ISO 8601 format. The agent will trigger temporal scoping routines to expose specific documents mapped historically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/granola](https://vinkius.com/mcp/granola)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Granola** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `granola` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Granola** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "granola": {
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
