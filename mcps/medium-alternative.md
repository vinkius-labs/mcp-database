# Medium MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/medium-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/medium-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/medium-alternative-mcp)
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


## Available Tools
- **create_post**: Create a new post on Medium
- **create_publication_post**: Create a new post under a publication
- **get_me**: Get authenticated user info from Medium
- **list_contributors**: List publication contributors
- **list_publications**: List user publications


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


## Installation & Usage

To install and use the **Medium** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/medium-alternative](https://vinkius.com/mcp/medium-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
