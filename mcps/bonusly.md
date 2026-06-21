# Bonusly MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bonusly)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bonusly-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bonusly-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Recognize and reward your team via Bonusly — give bonuses, track points, and view leaderboards directly from any AI agent.

## Description
Connect your **Bonusly** employee recognition account to any AI agent and orchestrate your team culture and reward workflows through natural conversation.

### What you can do

- **Peer Recognition** — Instantly give bonuses to colleagues with custom reasons and hashtags representing company values.
- **Bonus Oversight** — List recent bonuses and retrieve detailed information for specific recognition events.
- **User & Profile Management** — Access employee profiles and check your own point balance and history.
- **Reward Tracking** — Monitor recent redemptions to see how your team is spending their earned points.
- **Culture Insights** — List company values, popular hashtags, and view the real-time recognition leaderboard.

### How it works

1. Subscribe to this server
2. Enter your Bonusly API Access Token
3. Start rewarding your team from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Team Leads** — quickly recognize members for great work without leaving their workflow tools.
- **HR Managers** — monitor employee engagement and company value alignment using natural language.
- **Employees** — check their point balances and give quick shout-outs to peers.


## Available Tools
- **get_bonus**: Get details of a specific bonus
- **get_leaderboard**: Get the recognition leaderboard
- **get_my_profile**: Get the profile of the authenticated user
- **get_user**: Get profile details for an employee
- **give_bonus**: Give a recognition bonus to an employee
- **list_bonuses**: List recent employee bonuses
- **list_hashtags**: List popular hashtags
- **list_redemptions**: List recent reward redemptions
- **list_users**: List all employees
- **list_company_values**: List company values and hashtags


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bonusly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give +10 to sarah@example.com for helping with the client presentation #teamwork."

**🤖 AI Agent:**
> Recognition posted! I've given 10 points to Sarah with the reason: 'helping with the client presentation #teamwork'.

---

**👤 You:**
> "What is my current Bonusly balance?"

**🤖 AI Agent:**
> You currently have 150 points available to give and 450 points that you've received and can redeem for rewards.

---

**👤 You:**
> "Show the recent bonuses in the company."

**🤖 AI Agent:**
> Retrieving recent bonuses... Notable recognition includes Mark giving to Alice for 'great code review' and Janet giving to the team for 'launching the new site'.


## Installation & Usage

To install and use the **Bonusly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bonusly](https://vinkius.com/mcp/bonusly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
