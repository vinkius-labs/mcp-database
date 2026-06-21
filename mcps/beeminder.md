# Beeminder MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/beeminder)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/beeminder-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/beeminder-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Commit to your goals via Beeminder — track progress, add datapoints, and monitor your road status directly from any AI agent.

## Description
Connect your **Beeminder** account to any AI agent and integrate goal tracking into your daily workflow through natural conversation.

### What you can do

- **Goal Oversight** — List and inspect all active goals to keep your commitments front and center.
- **Data Management** — Add, update, and delete datapoints for your goals to stay on your 'Yellow Brick Road'.
- **Status Monitoring** — Check real-time road status colors and 'limsum' summaries to avoid derailment.
- **Goal Refresh** — Trigger manual refreshes for your goals to ensure the latest data is reflected.
- **Charge Auditing** — List recent charges and pledges associated with your account.

### How it works

1. Subscribe to this server
2. Enter your Beeminder Username and Auth Token
3. Start minding your goals from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Self-Quantifiers** — instantly log metrics (e.g., words written, gym visits) without leaving your workspace.
- **Productivity Enthusiasts** — monitor goal statuses during daily standups or weekly reviews via the agent.
- **Developers** — automate datapoint logging from within the code editor or automated scripts.


## Available Tools
- **add_datapoint**: Add a new datapoint to a goal
- **delete_datapoint**: Delete a datapoint
- **get_goal_status**: Check the current status of a goal
- **get_goal**: Get specific goal details
- **get_user_info**: Get Beeminder user profile
- **list_charges**: List recent charges/pledges
- **list_datapoints**: List datapoints for a goal
- **list_goals**: List all active Beeminder goals
- **refresh_goal**: Trigger a refresh for a goal
- **update_datapoint**: Update an existing datapoint


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beeminder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active Beeminder goals."

**🤖 AI Agent:**
> I've retrieved your goals. You have 3 active goals: 'Gym' (slug: gym), 'Reading' (slug: books), and 'Coding' (slug: project-x). Would you like the status for any of these?

---

**👤 You:**
> "Log 500 words to my 'Reading' goal."

**🤖 AI Agent:**
> Done! I've added a datapoint of 500 to your 'Reading' goal (slug: books). Your road status is now green.

---

**👤 You:**
> "Check status for goal 'gym'."

**🤖 AI Agent:**
> The goal 'Gym' is currently yellow. You have 2 days until derailment. You need to add a datapoint soon to stay on the road!


## Installation & Usage

To install and use the **Beeminder** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/beeminder](https://vinkius.com/mcp/beeminder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
