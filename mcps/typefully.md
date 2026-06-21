# Typefully MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/typefully)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/typefully-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/typefully-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Write, schedule, and grow your audience on Twitter and LinkedIn with an editor that helps you craft threads that go viral.

## Description
Connect your **Typefully** account to any AI agent and simplify how you draft, schedule, and publish high-engagement content for X (Twitter) and LinkedIn through natural conversation.

### What you can do

- **Draft Management** — List all your content drafts and retrieve detailed text and settings for specific ideas.
- **Instant Publishing** — Post content immediately to all your enabled social platforms directly via AI commands.
- **Smart Scheduling** — Schedule your posts for a specific time or use the 'next-free-slot' feature to optimize your queue.
- **Account Directory** — List all connected social sets and brands managed in your Typefully workspace.
- **Draft Lifecycle** — Create, update, and delete drafts programmatically to maintain your content pipeline.
- **User Insights** — Retrieve your profile details and verify account configurations directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Typefully Personal API Key (found in your settings under API)
3. Start managing your social presence from Claude, Cursor, or any MCP client

### Who is this for?

- **Content Creators & Influencers** — quickly draft threads and schedule posts via simple AI commands.
- **Marketing Managers** — monitor content queues and publish updates across multiple brands directly from the workspace.
- **Social Media Teams** — coordinate draft reviews and optimize publishing times via the AI assistant.


## Available Tools
- **create_draft**: Create a new content draft
- **delete_draft**: Remove a draft
- **get_draft_details**: Get details for a draft
- **list_drafts**: List content drafts
- **list_social_accounts**: List connected social accounts
- **publish_immediately**: Publish content right now
- **schedule_content**: Schedule content for later
- **update_draft**: Modify an existing draft
- **get_user_profile**: Get your Typefully profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Typefully** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my social accounts in Typefully."

**🤖 AI Agent:**
> I've retrieved your social sets. You have 2 active brands: 'Personal Branding' (X + LinkedIn) and 'Company News'. Which one would you like to manage drafts for?

---

**👤 You:**
> "Publish this to my personal account now: 'Excited to announce our new MCP server! #AI #DevTools'"

**🤖 AI Agent:**
> Published! I've posted your content to all enabled platforms for your 'Personal Branding' account. Your post is now live.

---

**👤 You:**
> "Show me all scheduled drafts for the 'Company News' account."

**🤖 AI Agent:**
> I've fetched the scheduled content. You have 3 posts in the queue for 'Company News', including a thread for Tuesday and a single post for Friday. Would you like to review the text for any of them?


## Installation & Usage

To install and use the **Typefully** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/typefully](https://vinkius.com/mcp/typefully)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
