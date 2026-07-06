# Typefully MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/typefully)
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


## Available Tools (9)
- **list_social_accounts**: List connected social accounts
- **publish_immediately**: Publish content right now
- **schedule_content**: Schedule content for later
- **update_draft**: Modify an existing draft
- **get_user_profile**: Get your Typefully profile
- **create_draft**: Create a new content draft
- **delete_draft**: Remove a draft
- **get_draft_details**: Get details for a draft
- **list_drafts**: List content drafts


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


## ❓ FAQ

**Q: Can I publish to both X and LinkedIn at the same time?**
Yes! When using the `publish_immediately` tool, you can specify the target platform or let Typefully post to all enabled channels for that social set.

**Q: How do I schedule a post for the next available time slot?**
Use the `schedule_content` tool and set the `publishAt` parameter to 'next-free-slot'. Typefully will automatically place the post in the best upcoming time according to your queue settings.

**Q: Is it possible to see the content of an existing draft?**
Absolutely. Use the `get_draft_details` tool and provide the Social Set ID and Draft ID. The agent will retrieve the full text and configuration for that draft.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/typefully](https://vinkius.com/mcp/typefully)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Typefully** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `typefully` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Typefully** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "typefully": {
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
