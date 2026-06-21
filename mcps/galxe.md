# Galxe MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/galxe)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/galxe-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/galxe-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate Web3 community management via Galxe — check quest eligibility, track leaderboards, and manage credentials directly from any AI agent.

## Description
Connect your **Galxe** account to any AI agent to streamline your Web3 growth and community operations through natural conversation.

### What you can do

- **Quest Insights** — Fetch comprehensive details for specific Galxe quests, including status and participant data.
- **Eligibility Verification** — Instantly check if a wallet address is eligible for specific quests or credential groups.
- **Leaderboard Tracking** — Monitor loyalty points within spaces or track Twitter influence via Starboard metrics.
- **Credential Management** — Programmatically append, remove, or replace eligible users for custom API credentials.
- **Social Metrics** — Retrieve influence scores and social rankings to identify top community contributors.

### How it works

1. Subscribe to this server
2. Enter your Galxe Access Token
3. Start managing your Web3 campaigns from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Community Managers** — track participant progress and verify eligibility without manual dashboard exports.
- **Growth Leads** — analyze leaderboard data and social influence to optimize campaign targeting.
- **Web3 Developers** — automate the synchronization of eligible users for custom credentials directly from their workflow.


## Available Tools
- **check_credential_eligibility**: Check user eligibility for a specific credential
- **check_quest_eligibility**: Check user eligibility for a Galxe quest
- **get_quest**: Get Galxe quest details
- **get_space_leaderboard**: Get loyalty points leaderboard for a Galxe space
- **get_starboard_leaderboard**: Get Starboard leaderboard for Twitter influence
- **mutate_credential_items**: Modify eligible users for an API credential


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Galxe** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the details for Galxe quest ID 'GCabc123'."

**🤖 AI Agent:**
> I've retrieved the details for quest 'GCabc123'. It is currently 'Active' with 1,250 participants. The space associated is 'Web3 Pioneers'. Would you like to check eligibility for a specific address?

---

**👤 You:**
> "Check if wallet 0x123... is eligible for quest 'GCxyz789'."

**🤖 AI Agent:**
> Checking eligibility... The address 0x123... is currently eligible for quest 'GCxyz789'. All required credential groups have been satisfied.

---

**👤 You:**
> "Show me the top 10 users on the leaderboard for space ID 555."

**🤖 AI Agent:**
> Fetching space leaderboard... Here are the top users for Space 555: 1. UserA (5000 pts), 2. UserB (4850 pts), 3. UserC (4700 pts)... Would you like to see more entries?


## Installation & Usage

To install and use the **Galxe** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/galxe](https://vinkius.com/mcp/galxe)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
