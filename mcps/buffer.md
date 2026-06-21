# Buffer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/buffer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate social media management via Buffer — schedule posts, track sent updates, shuffle queues, and manage multi-platform profiles with any AI agent.

## Description
Connect your **Buffer** account to any AI agent and take full control of your social media scheduling operations across Twitter, LinkedIn, Facebook, and Instagram through natural conversation.

### What you can do

- **Post Generation & Scheduling** — Allow your agent to draft, format, and immediately schedule cross-platform posts
- **Queue Management** — Review your pending scheduled posts, shuffle their order, or delete drafts before they go live
- **Performance Tracking** — Retrieve historical data for sent updates, summarizing click and engagement metrics
- **Profile Insights** — Check all connected social accounts, their IDs, and the precise timeslot schedules allocated to them
- **Status Validation** — Query specific pending updates by ID to review text, media attachments, and exact airtimes

### How it works

1. Subscribe to this server
2. Enter your Buffer API Token
3. Start ideating and scheduling tweets/posts directly from Claude, Cursor, or any MCP-compatible client

No more switching tabs to copy-paste generated tweets. Your AI is now officially your publishing engine.

### Who is this for?

- **Social Media Managers** — have your agent draft 10 tweets based on a blog post and instantly queue them to your Buffer
- **Founders & Creators** — review your queued content for the week without leaving your favorite coding/writing environment
- **Marketing Teams** — pull a summary of last week's sent posts' engagement directly into your strategy session chats


## Available Tools (10)
- **list_profiles**: List all connected social profiles
- **get_config**: Get supported services configuration
- **get_profile**: Get social profile details
- **list_pending_updates**: List scheduled posts awaiting publication
- **list_sent_updates**: List published posts
- **create_update**: Supports text, links, and auto-shortening.

Schedule a new social media post
- **delete_update**: Delete a scheduled post
- **reorder_updates**: Reorder scheduled posts
- **shuffle_updates**: Shuffle the post queue randomly
- **get_user**: Get Buffer account info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Buffer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my social media profiles currently connected to Buffer."

**🤖 AI Agent:**
> You have 2 profiles connected to your Buffer account:
1. Twitter (@TechVinkius) — Profile ID: 62a3f... 
2. LinkedIn (Vinkius Labs Page) — Profile ID: 61e9b...

Should I check the pending queue for any of these?

---

**👤 You:**
> "How many pending posts do I have on my Twitter account?"

**🤖 AI Agent:**
> You currently have 3 pending posts scheduled for Twitter (@TechVinkius). 
The next one is scheduled to go live today at 14:00 GMT: "Understanding MCP architecture unlocks pure agentic scale..." 

Would you like me to shuffle them or create a new one?

---

**👤 You:**
> "Write a short engaging tweet about our new launch and schedule it immediately."

**🤖 AI Agent:**
> Drafted: "🚀 Boom! We just shipped the final feature set for our platform! The future of agentic ecosystems is live. #agents #ai"

I have successfully injected this into the Buffer queue for your Twitter profile (ID: 62a3f). It will automatically take the next available time slot according to your predefined buffer schedule.


## ❓ FAQ

**Q: Can my AI draft a post and immediately schedule it?**
Yes! The `create_update` tool is specifically designed for this. You can list your profiles to fetch the correct profile IDs, and then instruct the agent to write a post. The agent will push the new content using the IDs as target destinations. If you omit the explicit time, it falls back to the next empty spot in the profile's schedule.

**Q: Can the agent shuffle my pending queue if I don't like the order?**
Yes. If you have loaded 20 evergreen posts into your Buffer, you can simply ask the agent to "shuffle the queue for my Twitter profile." It will invoke the `shuffle_queue` endpoint to mix up all pending un-timed updates, keeping your timeline fresh.

**Q: Is there a risk that my AI posts something to the wrong account?**
The integration mandates profile IDs explicitly inside the payload. As a safety net, always instruct your AI to *list* your pending posts and verify the target profile string names *before* pulling the trigger on production updates. The agent behaves deterministically with tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/buffer](https://vinkius.com/mcp/buffer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Buffer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `buffer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Buffer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "buffer": {
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
