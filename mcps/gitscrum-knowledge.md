# GitScrum Knowledge MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gitscrum-knowledge)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Build and query knowledge bases via GitScrum — manage notes as agent memory, maintain wiki pages, communicate through discussions, and search across all resources from any AI agent.

## Description
### What you can do

- **Agent memory via notes** — create, update, share, and organize notes as persistent AI memory with full revision history and folder management
- **Wiki knowledge base** — build and maintain project documentation with nested pages, markdown content, revision tracking, and restore capabilities
- **Team discussions** — create channels, send messages, search conversations, and reply in threads for structured team communication
- **Global search** — search across tasks, wiki pages, discussions, user stories, sprints, and notes in a single query
- **Knowledge versioning** — track how information evolves over time with note and wiki revision histories

### How it works

1. Subscribe to the GitScrum Knowledge integration from the marketplace
2. Enter your GitScrum API token and company slug
3. Use your agent as a knowledge hub — store decisions in notes, document processes in wiki, discuss with the team, and search everything in natural language

Your agent becomes the central knowledge repository, bridging personal memory with team knowledge.

### Who is this for?

- **AI practitioners** — maintain persistent agent memory across sessions using notes as structured context
- **Technical writers** — manage wiki documentation with version control and search directly through conversation
- **Team leads** — foster asynchronous team communication and decision-tracking without platform switching


## Available Tools
- **create_channel**: Create a discussion channel
- **get_channel**: Get channel details
- **list_channels**: List discussion channels
- **list_discussions**: List all discussions in a project
- **create_note_folder**: E.g., "Agent Memory", "Architecture Decisions", "Meeting Notes".

Create a note folder
- **list_note_folders**: Use folders to categorize agent memory by topic or project.

List note folders
- **rename_note_folder**: Rename a note folder
- **channel_messages**: Get messages in a channel
- **search_channel_messages**: Search messages in a channel
- **send_message**: Useful for agents to communicate findings or status updates.

Send a message to a channel
- **create_note**: Use this as persistent agent memory: store decisions, context, meeting notes, or ADRs. Content supports full markdown.

Create a new note
- **delete_note**: Delete a note permanently
- **list_notes**: Perfect for agent memory — store context, decisions, and key information across sessions.

List all notes in the workspace
- **move_note_to_folder**: Move a note into a folder
- **note_revisions**: Useful for tracking how knowledge evolved over time.

Get note revision history
- **toggle_note_share**: Useful for publishing agent findings to the team.

Toggle note sharing visibility
- **update_note**: Use to append context or refine agent memory over time.

Update an existing note
- **reply_to_message**: Reply to a message in a thread
- **global_search**: Returns grouped results by resource type.

Search across all workspace resources
- **thread_replies**: Get thread replies for a message
- **create_wiki_page**: Supports nested pages via parent_uuid.

Create a wiki page
- **delete_wiki_page**: Delete a wiki page
- **get_wiki_page**: Get a wiki page with full content
- **list_wiki_pages**: Wiki pages support markdown and nested hierarchies.

List wiki pages in a project
- **restore_wiki_revision**: Restore a wiki page to a previous revision
- **wiki_revisions**: Get wiki page revision history
- **search_wiki**: Search wiki pages
- **update_wiki_page**: Update a wiki page


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GitScrum Knowledge** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Save a note with today's architecture decision about using event sourcing."

**🤖 AI Agent:**
> Note created: 'ADR-007: Event Sourcing for Order Service' with your decision rationale in markdown. I've placed it in the 'Architecture Decisions' folder. The note is private — say 'share this note' when you're ready to publish it to the team.

---

**👤 You:**
> "Search everything in our workspace for 'payment gateway integration'."

**🤖 AI Agent:**
> Found 11 results across your workspace: 📋 3 tasks (WEB-28, WEB-31, WEB-40), 📚 2 wiki pages ('Payment Flow Architecture', 'Gateway Comparison'), 💬 4 discussion messages in #payments channel, 📝 2 notes ('Payment Provider Research', 'Stripe vs Adyen Analysis'). Want me to open any of these?

---

**👤 You:**
> "Post an update in the #engineering channel about today's deployment."

**🤖 AI Agent:**
> Message posted to #engineering: '🚀 Deployment complete — v2.4.1 is now live in production. Key changes: payment gateway integration, performance optimizations, and 3 bug fixes. Full changelog in the wiki.' The team will be notified. Want me to create a wiki page with the detailed changelog?


## ❓ FAQ

**Q: Can my AI agent use notes as persistent memory across sessions?**
Absolutely — this is a core design goal. Use `create_note` to store decisions, context, or meeting summaries as markdown notes. Organize them into folders with `create_note_folder` and `move_note_to_folder`. Use `toggle_note_share` to publish findings to the team. Every edit is versioned via `note_revisions` so you can track how knowledge evolves.

**Q: Can the agent search across everything in my workspace at once?**
Yes! The `global_search` tool performs a unified search across tasks, wiki pages, discussions, user stories, sprints, and notes. Results are grouped by resource type, so you instantly see where every mention lives. It's the fastest way to find anything in your workspace.

**Q: Can the agent participate in team discussions and reply to threads?**
Yes. Use `send_message` to post updates to any discussion channel, and `reply_to_message` for threaded conversations. The agent can also create channels with `create_channel`, search message history with `search_channel_messages`, and review thread replies with `thread_replies` — enabling fully automated status updates and knowledge sharing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gitscrum-knowledge](https://vinkius.com/mcp/gitscrum-knowledge)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GitScrum Knowledge** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gitscrum-knowledge` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GitScrum Knowledge** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gitscrum-knowledge": {
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
