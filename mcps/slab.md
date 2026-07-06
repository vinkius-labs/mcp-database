# Slab MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/slab)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Manage your team's knowledge base — query wiki articles, create new documentation, and explore topics directly using AI agents.

## Description
Connect your **Slab** workspace to any AI agent and empower your team to search, read, and write documentation seamlessly. Interact with your organization's entire knowledge base through natural language without ever switching tabs.

### What you can do

- **Deep Search & Retrieval** — Execute full-text searches across all Slab posts to fetch answers, guidelines, and protocols instantly
- **Documentation Authoring** — Create new articles, meeting notes, or project specs in Markdown, and update existing posts on the fly
- **Information Architecture** — Browse all your topics (folders) to understand how the company wiki is structured and fetch categorized articles
- **Activity Feeds** — Pull the most recently updated posts to stay on top of new company policies and documentation changes
- **Team Discovery** — Retrieve organization metadata and list all registered team members

### How it works

1. Subscribe to this server
2. Enter your Slab Access Token
3. Start using Claude, Cursor, or any MCP-compatible client to query your company's collective brain

Stop interrupting engineers to ask where a specific document lives. Your AI agent can read the internal wiki and answer questions directly based on your approved Slab content.

### Who is this for?

- **Software Developers** — pull API documentation or architectural guidelines directly into your IDE while coding
- **Product Managers** — instantly draft and publish feature specifications or release notes to the right Slab topic
- **Onboarding & HR** — ask your assistant to fetch the latest company policies or generate reading lists for new hires


## Available Tools (12)
- **get_topic_details**: Retrieve details and list of posts for a specific Slab topic
- **list_users**: List all members of the Slab organization
- **get_organization**: Retrieve the Slab organization profile
- **create_post**: Provide content in Markdown.

Create a new wiki post in Slab
- **update_post**: Update an existing Slab post title or content
- **create_topic**: Create a new topic in Slab to organize posts
- **archive_post**: This action is irreversible via API.

Archive an existing Slab post
- **list_recent_posts**: List the most recently updated posts
- **list_posts**: Returns post IDs and titles.

List all wiki posts/articles in the Slab workspace
- **get_post_details**: Retrieve the full content and metadata of a specific Slab post
- **search_posts**: Full-text search across all Slab posts
- **list_topics**: List all topics organizing posts in the Slab workspace


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Slab** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search the Slab wiki for 'VPN Setup Instructions'."

**🤖 AI Agent:**
> I found a match in your Slab knowledge base:
**Post Title**: 'Connecting to the Corporate VPN (macOS & Windows)'
**Post ID**: `p-1a2b3c4`
**Snippet**: '...to access staging environments, you must connect via the AnyConnect Client. Use your Okta credentials...'

Would you like me to retrieve the complete article so you can read the step-by-step instructions?

---

**👤 You:**
> "Create a new topic named 'Q3 Planning' and list the ID so I can save posts to it."

**🤖 AI Agent:**
> I've successfully created the new topic in Slab.
**Name**: Q3 Planning
**Topic ID**: `t-987xyzw`

Your topic is ready. Whenever we draft notes or objectives in this chat, just tell me to save them into `t-987xyzw`.

---

**👤 You:**
> "List the most recent 5 posts updated in the company wiki."

**🤖 AI Agent:**
> Here are the 5 most recently updated Slab posts across your organization:
1. Update: Engineering Sprint 42 (Updated 10 mins ago)
2. [DRAFT] Series B Milestones (Updated 2 hours ago)
3. Employee Onboarding Guide (Updated yesterday)
4. Q2 Architecture Diagrams (Updated yesterday)
5. Security Incident Playbook (Updated Monday)

Let me know if you need to read the full contents of any of these updates.


## ❓ FAQ

**Q: Can my AI use existing wiki guidelines to write new code or copy?**
Absolutely. You can request your agent to 'search the Slab wiki for our Frontend Coding Standards' or 'find our Brand Voice Guidelines'. The agent will retrieve the exact Markdown content of those articles and use them as system instructions for the rest of your conversation.

**Q: How do I easily publish my AI chat output back to Slab?**
When your AI agent generates a good technical specification or summary, simply tell it: 'Create a new post in Slab called [Name], using this entire response as the content, and place it in the Engineering topic.' The agent will format the Markdown and publish it immediately through the `create_post` tool.

**Q: Can my agent clean up outdated company documentation?**
Yes. If an article is deprecated, you can tell your AI: 'Archive the post with ID XYZ' or 'Find the old setup guide and archive it.' The agent can execute the `archive_post` command to hide outdated information and keep your knowledge base pristine.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/slab](https://vinkius.com/mcp/slab)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Slab** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `slab` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Slab** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "slab": {
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
