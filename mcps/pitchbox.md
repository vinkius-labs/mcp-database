# PitchBox MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pitchbox)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pitchbox-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pitchbox-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage influencer outreach and content marketing via PitchBox — list projects, track opportunities, and monitor emails directly from any AI agent.

## Description
Connect your **PitchBox** account to any AI agent and take full control of your outreach and link-building workflows through natural conversation.

### What you can do

- **Project & Campaign Oversight** — List all projects and campaigns to maintain visibility over your outreach efforts.
- **Opportunity Tracking** — List and retrieve detailed metadata for outreach opportunities (leads) within your campaigns.
- **Communication Monitoring** — List emails sent and received for any specific opportunity to understand the status of your pitches.
- **Contact Management** — List all contacts associated with an opportunity to manage your relationships effectively.
- **Task Visibility** — List active tasks across your account to stay on top of your daily operational needs.

### How it works

1. Subscribe to this server
2. Enter your PitchBox API Key (from account settings)
3. Start managing your outreach directly from Claude, Cursor, or any MCP client

### Who is this for?

- **SEO Specialists** — quickly check the status of a link-building opportunity or review recent emails while preparing reports.
- **Influencer Managers** — monitor campaign progress and contact details directly from your chat interface.
- **Content Marketers** — verify project metadata and pending tasks without leaving your workflow.


## Available Tools
- **get_pitchbox_campaign**: Get details for a specific campaign
- **get_pitchbox_me**: Get current user profile info
- **get_pitchbox_opportunity**: Get details for a specific opportunity
- **get_pitchbox_project**: Get details for a specific project
- **list_pitchbox_campaigns**: List campaigns in a project
- **list_pitchbox_contacts**: List contacts for an opportunity
- **list_pitchbox_emails**: List emails sent for an opportunity
- **list_pitchbox_opportunities**: List outreach opportunities (leads) in a campaign
- **list_pitchbox_projects**: List all PitchBox projects
- **list_pitchbox_tasks**: List active tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PitchBox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active campaigns in my 'Guest Posting' project."

**🤖 AI Agent:**
> I've retrieved your campaigns. In the 'Guest Posting' project, you have 4 active ones: 'Tech Blogs Q4', 'Lifestyle Outlets', 'Marketing Insights', and 'Industry News'.

---

**👤 You:**
> "Show me the status of the link-building opportunity for 'example.com'."

**🤖 AI Agent:**
> The opportunity for 'example.com' (ID: 98765) is currently in the 'Replied' stage. A follow-up email was sent 2 days ago. Would you like to see the last email message?

---

**👤 You:**
> "What outreach tasks are assigned to me for today?"

**🤖 AI Agent:**
> You have 5 tasks for today: 'Review pitches for Campaign 123', 'Verify contact for Opp 456', and 3 personalization tasks. Would you like to start with the reviews?


## Installation & Usage

To install and use the **PitchBox** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pitchbox](https://vinkius.com/mcp/pitchbox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
