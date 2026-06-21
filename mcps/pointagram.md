# Pointagram MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pointagram)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pointagram-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pointagram-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Motivate your sales team with gamified leaderboards, competitions, and rewards that turn KPIs into engaging daily challenges.

## Description
Connect your **Pointagram** account to any AI agent to streamline your team gamification and engagement workflows. Pointagram provides a powerful platform for programmatically managing players, teams, and score series through its robust v2.0 REST API.

### What you can do

- **Player Orchestration** — List and create player profiles with detailed tracking of levels, nicknames, and avatars
- **Scoring Event Automation** — Post real-time scoring events to update player points across different score series programmatically
- **Team Management** — Access and monitor your gamification teams and retrieve detailed membership metadata
- **Score Series Discovery** — List all your active score series to understand how points are accumulated and distributed
- **Performance Intelligence** — Retrieve granular player stats and rankings using natural language commands

### How it works

1. Subscribe to this server
2. Enter your Pointagram API Key and API User (email) from your dashboard settings
3. Start managing your gamification data from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales Managers & HR** — monitor team performance and trigger gamified rewards using natural language
- **Engagement Specialists** — automate the recognition of employee achievements more efficiently
- **Developers** — integrate real-time gamification data and player stats into custom business dashboards


## Available Tools
- **create_player**: Pass data as a JSON string.

Create a new player
- **get_player_stats**: Get stats for a player
- **list_players**: List all Pointagram players
- **list_score_series**: List all score series
- **list_teams**: List all Pointagram teams
- **post_event**: Pass data as a JSON string.

Post a scoring event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pointagram** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active players in Pointagram."

**🤖 AI Agent:**
> I've retrieved your player list. You have 50 active participants, including 'John Doe' (Level 12) and 'Maria Garcia' (Level 15). Would you like to see the stats for any of them?

---

**👤 You:**
> "Post 100 points for player '123' in the 'Sales Bonus' series."

**🤖 AI Agent:**
> Points posted successfully! I've added 100 points to player '123' in the 'Sales Bonus' series. The leaderboard will be updated shortly.

---

**👤 You:**
> "Show me the top 5 score series."

**🤖 AI Agent:**
> I've retrieved your score series. Your top active series include 'Monthly Sales Target', 'Customer Support Excellence', and 'Bug Squashing Challenge'. Which one would you like to explore?


## Installation & Usage

To install and use the **Pointagram** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pointagram](https://vinkius.com/mcp/pointagram)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
