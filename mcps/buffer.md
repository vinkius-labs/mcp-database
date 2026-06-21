# Buffer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/buffer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/buffer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/buffer-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Buffer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/buffer](https://vinkius.com/mcp/buffer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
