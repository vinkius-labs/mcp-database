# Medium MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/medium-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage your Medium profile — publish stories, audit publications, and contributors via AI.

## Description
Empower your AI agent to orchestrate your entire writing ecosystem on **Medium**, the platform for world-class stories and ideas. By connecting Medium to your agent, you transform publishing into a natural conversation. Your agent can instantly list your publications, audit contributor lists, and create new posts without you ever touching a dashboard. Whether you are a solo blogger or managing a high-traffic publication, your agent acts as a real-time editorial assistant, ensuring your content is always correctly formatted and distributed.

### What you can do

- **Post Distribution** — Create and publish new stories directly to your profile or a target publication with custom tags.
- **Publication Auditing** — List all publications associated with your account and retrieve detailed metadata for each.
- **Contributor Oversight** — Query contributor lists for any publication to maintain a clear view of your writing team.
- **Profile Intelligence** — Retrieve detailed user information and username details to ensure organizational alignment.
- **Content Formatting** — Publish content in both HTML and Markdown to maintain your desired aesthetic.

### How it works

1. Subscribe to this server
2. Enter your Medium Integration Token
3. Start managing your publishing workflow through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — publish drafts and stories straight from your writing workflow.
- **Editors** — verify contributor lists and audit publication statuses without manual logins.
- **Marketing Teams** — perform rapid audits of published content and manage tag strategies through natural language.
- **Operations Leads** — automate publishing querying to orchestrate cross-functional editorial teams smoothly.


## Available Tools (5)
- **list_contributors**: List publication contributors
- **list_publications**: List user publications
- **create_post**: Create a new post on Medium
- **create_publication_post**: Create a new post under a publication
- **get_me**: Get authenticated user info from Medium


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Medium** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get my Medium user ID and publications."

**🤖 AI Agent:**
> I've retrieved your profile. Your user ID is '12345' and you contribute to 2 publications: 'The Startup' and 'AI Trends'. Which one would you like to explore?

---

**👤 You:**
> "Publish a draft titled 'My AI Story' with tags 'AI,Future'."

**🤖 AI Agent:**
> Draft created! 'My AI Story' is now saved in your Medium account with 2 tags. You can review and publish it from your dashboard whenever you're ready.

---

**👤 You:**
> "Who are the contributors for publication ID xxxx?"

**🤖 AI Agent:**
> I've found 3 contributors for that publication: 'Jane Doe', 'Marcus R.', and 'BotAssistant'. Would you like to see their profile URLs?


## ❓ FAQ

**Q: How do I find my Medium Integration Token?**
Log in to Medium on the web, go to **Settings** > **Security and apps** > **Integration tokens**, and generate a new token. Copy and paste it into the field below.

**Q: Can the agent publish a story as a draft?**
Yes. When using the `create_post` tool, you can specify `draft` in the `publishStatus` parameter. Your agent will confirm that the story is saved as a draft for your review.

**Q: Is it possible to publish to a publication I contribute to?**
Yes. First, list your publications using `list_publications`, then use the `create_publication_post` tool with the target Publication ID to submit your story.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/medium-alternative](https://vinkius.com/mcp/medium-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Medium** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `medium-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Medium** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "medium-alternative": {
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
