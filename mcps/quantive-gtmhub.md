# Quantive (Gtmhub) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/quantive-gtmhub)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/quantive-gtmhub-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/quantive-gtmhub-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate OKR strategy via Quantive — manage objectives, key results, and sessions directly from any AI agent.

## Description
Connect your **Quantive** (formerly Gtmhub) strategy platform to any AI agent and drive your organizational goals through natural conversation.

### What you can do

- **Objective Tracking** — List and inspect strategic objectives to align your team's focus.
- **Key Result Management** — Monitor progress on KRs and update current values directly from your chat or IDE.
- **Session Overview** — Browse planning sessions and timeframes to understand quarterly or annual goals.
- **Team & User Insights** — Retrieve team structures and user profiles to facilitate better collaboration.
- **Task Execution** — List tasks linked to specific OKRs to bridge the gap between strategy and execution.

### How it works

1. Subscribe to this server
2. Enter your Quantive API Token and select your Data Center (US or EU)
3. Start managing your OKRs from Claude, Cursor, or any MCP-compatible client

Bridge the gap between your daily work and high-level strategy. Your AI assistant acts as a proactive strategy officer or OKR coach.

### Who is this for?

- **Product & Engineering Leaders** — keep track of sprint goals and KRs without leaving your development environment.
- **Operations Managers** — automate the collection of progress updates from various teams and sessions.
- **Strategy Officers** — maintain a real-time overview of organizational alignment and goal attainment.


## Available Tools
- **get_key_result**: Get details for a specific key result
- **get_my_profile**: Get information about the current authenticated user
- **get_objective**: Get details for a specific OKR objective
- **list_key_results**: List all key results (metrics) in Quantive
- **list_objectives**: List all OKR objectives in Quantive (Gtmhub)
- **list_sessions**: g., Q1, Annual) used to group OKRs.

List all planning sessions (timeframes) in Quantive
- **list_tasks**: List tasks associated with OKRs
- **list_teams**: List all organizational teams
- **list_users**: List user profiles in the Quantive account
- **update_key_result**: Update the current value of a key result


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Quantive (Gtmhub)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are our main objectives for the current session?"

**🤖 AI Agent:**
> I've retrieved your objectives. Currently, you have 3 active goals: 'Increase Market Share by 15%', 'Launch Version 2.0 of our Mobile App', and 'Improve Customer Retention to 90%'. Which one would you like to check progress on?

---

**👤 You:**
> "Update key result ID 593021 to 75."

**🤖 AI Agent:**
> Updating progress... Key Result 593021 has been successfully updated to 75. This brings the current attainment for this KR to 82.5%.

---

**👤 You:**
> "List all teams assigned to our strategic objectives."

**🤖 AI Agent:**
> I've fetched the team list. Your organizational OKRs are currently being driven by: 'Engineering Alpha', 'Product Design', 'Growth Marketing', and 'Customer Success'. Would you like to see the specific OKRs for any of these teams?


## Installation & Usage

To install and use the **Quantive (Gtmhub)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/quantive-gtmhub](https://vinkius.com/mcp/quantive-gtmhub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
