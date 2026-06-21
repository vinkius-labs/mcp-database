# Officevibe MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/officevibe)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/officevibe-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/officevibe-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage employee engagement via Officevibe — track pulse survey scores, feedback, and NPS directly from your AI agent.

## Description
Connect your **Officevibe** (by Workleap) account to your AI agent and gain deep insights into your workplace culture and employee engagement through natural conversation.

### What you can do

- **Engagement Scores** — Retrieve aggregated engagement and satisfaction scores for your entire organization or specific teams.
- **Pulse Metrics** — Access granular scores for key sub-metrics like Recognition, Relationship with Manager, and Wellness.
- **Feedback Monitoring** — List qualitative survey feedback and comments, and retrieve full follow-up conversations.
- **NPS Tracking** — Monitor your current Employee Net Promoter Score (eNPS) and view historical trends.
- **User & Team Oversight** — List all employees and organization segments to understand your culture's structure.
- **Deep Inspection** — Fetch complete metadata and profile information for specific employees using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your Officevibe API Key (generated in the Workleap Developer Portal)
3. Start monitoring your workplace culture from Claude, Cursor, or any MCP client

### Who is this for?

- **HR Managers & People Ops** — quickly check engagement trends or read recent feedback without opening the dashboard.
- **Team Leads & Supervisors** — monitor your team's pulse metrics and follow up on feedback in real-time.
- **Culture Officers** — automate the retrieval of NPS and engagement data for internal culture reporting.


## Available Tools
- **get_engagement_metrics**: g., Recognition, Relationship with Manager).

Get granular engagement metrics
- **get_engagement_scores**: Get overall engagement scores
- **get_feedback_replies**: Get feedback conversation
- **get_nps_scores**: Get employee NPS scores
- **get_employee_details**: Get specific employee info
- **list_user_attributes**: List custom user attributes
- **list_survey_feedback**: List survey feedback
- **list_vibe_segments**: List audience segments
- **list_vibe_teams**: List organization teams
- **list_employees**: List all employees


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Officevibe** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current organization engagement score?"

**🤖 AI Agent:**
> Retrieving engagement scores... Your organization's current engagement score is 8.2 out of 10. The score has remained stable over the last 30 days. Would you like a breakdown of the 10 key sub-metrics?

---

**👤 You:**
> "List the latest qualitative feedback from employee surveys."

**🤖 AI Agent:**
> Fetching survey feedback... I found 5 recent comments. One employee suggested 'More healthy snacks in the breakroom' while another mentioned 'Excellent support from my manager during the launch'. Shall I retrieve the full conversation for any of these?

---

**👤 You:**
> "Show me the Employee NPS (eNPS) trend for this quarter."

**🤖 AI Agent:**
> Retrieving NPS data... Your current eNPS is +45, which is considered 'Excellent'. The trend shows a steady climb from +38 at the beginning of the quarter. Would you like to see which team segment contributed most to this growth?


## Installation & Usage

To install and use the **Officevibe** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/officevibe](https://vinkius.com/mcp/officevibe)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
