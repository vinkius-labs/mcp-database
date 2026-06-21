# Roblox Social & Group Intelligence MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/roblox-social-group-intelligence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/roblox-social-group-intelligence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/roblox-social-group-intelligence-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

The definitive server for the Roblox social graph — track user profiles, friend lists, and group rankings via AI.

## Description
Equip your AI agent with deep intelligence for the **Roblox Social & Economy** ecosystem. This advanced MCP server provides high-precision access to official user metadata, social connections, and group organizational structures. Your agent can instantly resolve usernames into unique UserIDs, audit public friend lists, monitor real-time presence to see which games users are playing, and retrieve complete metadata for Roblox groups. Whether you are a community manager auditing organization rosters or a gamer tracking social reputation, your agent acts as a professional social data engineer through natural conversation.

### What you can do

- **Social Profiling** — Resolve usernames and retrieve unique AccountIDs, biographical metadata, and public status logs
- **Graph Intelligence** — Fetch official friend lists and follower counts to analyze social networks within the ecosystem
- **Presence Monitoring** — Retrieve real-time 'In-Game' or 'Online' status for multiple users simultaneously
- **Group Auditing** — Access official group metadata including member counts, rank structures, and ownership information

### How it works

1. Subscribe to this server
2. No API key required for public social discovery
3. Start managing your Roblox social intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Community Managers** — instantly monitor group growth and member activity directly from your workflow
- **Organizers & Scouts** — perform deep audits of player connections and organization rosters for competitive recruitment
- **Analytical Gamers** — track your social circle and presence status with micro-metric precision


## Available Tools
- **get_user_followers**: List followers of a Roblox user
- **get_user_followings**: List users followed by a Roblox user
- **get_user_friends**: List friends for a Roblox user
- **get_group_details**: Get details for a Roblox group
- **get_group_roles**: List all ranks and roles within a group
- **get_users_online_status**: Check if multiple users are online or in-game
- **get_user_badges**: List badges earned by a Roblox user
- **get_user_profile**: Get full profile for a Roblox user by ID
- **search_roblox_user**: Find Roblox users by username


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Roblox Social & Group Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the UserID for the Roblox user 'Builderman' and show his friend list."

**🤖 AI Agent:**
> Resolving username... I've found the account for 'Builderman' (ID: 156). I've also retrieved his public friend list which includes 68 users. Would you like to see his current presence status or account history?

---

**👤 You:**
> "Analyze the group ID '1' and list all available ranks and the owner."

**🤖 AI Agent:**
> Inspecting group metadata... Group ID '1' (Roblox) is owned by 'Builderman'. It has over 2 million members. I've retrieved the rank structure including 'Member', 'Moderator', and 'Admin'. Would you like the full list of members in a specific rank?

---

**👤 You:**
> "Check if user IDs '123, 456, 789' are currently playing any game together."

**🤖 AI Agent:**
> Running batch presence check... Users 123 and 456 are currently in the same experience: 'Work at a Pizza Place'. User 789 is currently offline. Shall I continue monitoring their status for any changes?


## Installation & Usage

To install and use the **Roblox Social & Group Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/roblox-social-group-intelligence](https://vinkius.com/mcp/roblox-social-group-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
