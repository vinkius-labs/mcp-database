# Salesforce Chatter MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/salesforce-chatter)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/salesforce-chatter-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/salesforce-chatter-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Read your Chatter feed, post messages, search groups, comment on posts, and collaborate across your Salesforce org through natural conversation.

## Description
Connect **Salesforce Chatter** to any AI agent.

### What you can do
- **Feed** — View your personalized news feed
- **Post** — Share updates on your feed or any record/group
- **Groups** — Search and browse Chatter groups
- **Comments** — Reply to any Chatter post

### Who is this for?
- **Sales Teams** — Share deal updates without opening Salesforce
- **Managers** — Stay informed on team activity
- **All Users** — Internal comms through your AI assistant


## Available Tools
- **sf_comment_on_post**: Requires the feed element ID.

Comment on a Chatter post
- **sf_chatter_feed**: Get the latest Chatter news feed for the authenticated user
- **sf_group_feed**: Requires the group ID (get from sf_search_chatter_groups).

Get the feed of a specific Chatter group
- **sf_post_to_chatter**: Provide parentId to post on a specific record.

Post a message to Chatter
- **sf_search_chatter_groups**: Returns group name, description, member count, visibility, and owner.

Search Chatter groups by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salesforce Chatter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is new on my Chatter feed?"

**🤖 AI Agent:**
> 📰 **Your Feed**
1. 👤 Sarah — "Q1 results are in — 23% above target!" (5 likes, 3 comments)
2. 👤 Marketing Team — New campaign launched (2 likes)
3. 👤 John — Deal closed: Acme Corp $50K (12 likes, 8 comments)

---

**👤 You:**
> "Post to Chatter: Great quarter everyone! Let us keep the momentum going."

**🤖 AI Agent:**
> ✅ **Posted!**
- "Great quarter everyone! Let us keep the momentum going."
- Posted to: My Feed

---

**👤 You:**
> "Find the Sales Team group on Chatter"

**🤖 AI Agent:**
> 👥 **Sales Team** — 45 members | Public
"Central hub for sales team updates, wins, and strategy discussions."
Last post: 2 hours ago


## Installation & Usage

To install and use the **Salesforce Chatter** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salesforce-chatter](https://vinkius.com/mcp/salesforce-chatter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
