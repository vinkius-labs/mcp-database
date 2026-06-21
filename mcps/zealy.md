# Zealy MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zealy)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zealy-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zealy-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Automate community growth and engagement on Zealy — manage quests, track leaderboards, and reward users directly from your AI agent.

## Description
Connect your **Zealy** community to any AI agent to streamline your Web3 and community marketing workflows. Take full control of your gamification strategy through natural conversation.

### What you can do

- **User & Membership** — Fetch detailed user profiles, search for members via Discord or ETH addresses, and verify community membership instantly.
- **XP & Gamification** — Manually add or remove XP from users, manage referral codes, and monitor real-time leaderboards to identify top contributors.
- **Quest Management** — List, create, and update quests, modules, and sprints to keep your community active and engaged.
- **Submission Reviews** — List and process quest submissions, allowing your AI to act as a community moderator by reviewing or approving tasks.
- **Webhooks & Automation** — Configure and manage webhooks to sync Zealy events with your external tools and databases.

### How it works

1. Subscribe to this server
2. Enter your Zealy API Key
3. Start managing your community growth from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Community Managers** — instantly reward contributors, review submissions, and check leaderboard standings without manual dashboard navigation.
- **Growth Marketers** — automate quest creation and track referral performance to optimize acquisition funnels.
- **Web3 Developers** — integrate community data and membership checks directly into your development workflow.


## Available Tools
- **get_review**: Retrieve a specific review by ID
- **get_user**: Fetch user details by Zealy ID
- **list_modules**: List all modules (categories) in a community
- **list_quests**: List all quests in a community
- **list_reviews**: Retrieve claimed quests waiting for review
- **list_secrets**: Fetches secrets configured for the community.

Retrieve community secrets used in API tasks
- **list_sprints**: Retrieve a list of community sprints
- **list_webhooks**: List all webhooks
- **remove_xp**: Manually remove XP from a user
- **review_submission**: Approve or reject claimed quests
- **search_users**: Search for users by social handles
- **update_quest**: Update an existing quest
- **update_webhook**: Update a webhook
- **add_xp**: Manually add XP to a user
- **ban_user**: Ban a user from the community
- **check_member**: Verify if a user belongs to a community
- **create_quest**: Create a new quest
- **create_secret**: Creates a new secret for the community.

Create a community secret for API tasks
- **create_webhook**: Create a webhook
- **delete_webhook**: Delete a webhook
- **get_community**: Retrieve basic information about a Zealy community
- **get_leaderboard**: Can be filtered by sprint.

Get the all-time or sprint leaderboard
- **get_referral_code**: Retrieve a user referral code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zealy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the user with Discord ID '123456789' in the 'my-community' subdomain."

**🤖 AI Agent:**
> I found the user! Their Zealy UUID is `abc-123-def`. They are currently Level 5 with 1,200 XP. Would you like to see their full profile?

---

**👤 You:**
> "Add 500 XP to user 'abc-123-def' in 'my-community' for 'Exceptional Content Creation'."

**🤖 AI Agent:**
> Successfully added 500 XP to the user. Their new total is 1,700 XP. The transaction has been logged with the label 'Exceptional Content Creation'.

---

**👤 You:**
> "List the top 5 users on the leaderboard for the 'my-community' subdomain."

**🤖 AI Agent:**
> Here are the top 5 contributors: 
1. UserA (5,000 XP)
2. UserB (4,850 XP)
3. UserC (4,200 XP)
4. UserD (3,900 XP)
5. UserE (3,750 XP)
Would you like to inspect any of these users specifically?


## Installation & Usage

To install and use the **Zealy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zealy](https://vinkius.com/mcp/zealy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
