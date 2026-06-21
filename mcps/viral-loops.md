# Viral Loops MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/viral-loops)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/viral-loops-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/viral-loops-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage referral campaigns, participants, milestones, and rewards via Viral Loops API.

## Description
Connect **Viral Loops** to any AI agent and supercharge your referral marketing — manage campaigns, track participants, monitor milestones, and analyze referral performance through natural conversation.

### What you can do
- **Campaign Management** — List and inspect all referral campaigns in your account
- **Participant Tracking** — View participants, their referral counts, and statuses
- **Referral URLs** — Generate and retrieve unique referral links for participants
- **Milestone Monitoring** — Check referral milestones and reward completion
- **Campaign Statistics** — Get performance metrics including total referrals and conversions
- **Reward Management** — View and manage reward configurations

### How it works
1. Subscribe to this server
2. Enter your Viral Loops API Key
3. Start managing referral campaigns from Claude, Cursor, or any MCP-compatible client

Viral Loops is the leading referral marketing platform used by thousands of businesses to grow through word-of-mouth.

### Who is this for?
- **Marketing Teams** — Monitor campaign performance and participant activity without logging into the dashboard
- **Growth Managers** — Track referral metrics and milestone completions in real-time
- **Customer Support** — Look up participant referral URLs and statuses quickly


## Available Tools
- **create_participant**: Use this when users sign up through your referral form.

Add a new participant to a referral campaign
- **get_campaign**: Use the campaign ID from list_campaigns.

Get detailed information about a specific campaign
- **get_milestones**: g., 5 referrals = discount, 10 referrals = free product) and their current completion status.

Get referral milestones and rewards for a campaign
- **get_participant**: Get details of a specific participant by email
- **get_referral_url**: Get the unique referral URL for a participant
- **get_rewards**: Get rewards configuration for a campaign
- **get_campaign_stats**: Get performance statistics for a campaign
- **list_campaigns**: Use this to discover available campaigns before querying specific ones.

List all referral campaigns in your Viral Loops account
- **list_participants**: Useful for leaderboard analysis and participant management.

List all participants in a referral campaign
- **update_participant**: Update information for an existing participant


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Viral Loops** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all my referral campaigns."

**🤖 AI Agent:**
> Found 3 campaigns: 1. Pre-Launch Waitlist (active). 2. Giveaway Campaign (active). 3. Milestone Rewards (draft).

---

**👤 You:**
> "Get the referral URL for user@example.com in campaign 123."

**🤖 AI Agent:**
> Referral URL: https://app.viral-loops.com/ref/abc123?email=user@example.com

---

**👤 You:**
> "Show me the stats for campaign 123."

**🤖 AI Agent:**
> Campaign Stats: 1,250 participants, 4,800 referrals, 320 conversions (25.6% conversion rate).


## Installation & Usage

To install and use the **Viral Loops** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/viral-loops](https://vinkius.com/mcp/viral-loops)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
