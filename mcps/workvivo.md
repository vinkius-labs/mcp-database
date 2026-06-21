# Workvivo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/workvivo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/workvivo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/workvivo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage social posts, employee profiles, and collaboration spaces on Workvivo — the employee experience platform.

## Description
Connect your **Workvivo** account to any AI agent and manage your employee experience infrastructure through natural conversation.

### What you can do

- **Social Feed** — Browse the company activity feed, retrieve full details for specific posts (likes, comments), and share new updates instantly
- **Employee Directory** — List all registered employees and retrieve comprehensive profile details including contact info and job titles
- **Collaboration Spaces** — Browse interest groups and departmental spaces, retrieve membership counts, and post updates to specific spaces
- **Company Events** — Monitor the company calendar, retrieve details for upcoming events including location and start times
- **Content Insights** — Quickly find unique post, employee, space, and event IDs required for automated internal communication workflows
- **Team Engagement** — Analyze activity levels and browse social interactions across the platform directly from your agent
- **Data Integrity** — Safely delete unfinalized or obsolete social posts through simple chat commands

### How it works

1. Subscribe to this server
2. Enter your Workvivo Domain and API Token
3. Start managing your internal communications through Claude, Cursor, or any MCP-compatible client

No more manual logging into the Workvivo dashboard to post a simple update. Your AI agent becomes your internal communications assistant.

### Who is this for?

- **Internal Comms Teams** — automate post publication and monitor feed activity through simple conversation
- **HR Managers** — browse employee profiles and manage collaboration spaces without manual navigation
- **Project Leads** — quickly share updates to specific project spaces and retrieve upcoming event details
- **Executive Assistants** — schedule company-wide announcements and verify event information through chat


## Available Tools
- **create_social_post**: Provide the text content and an optional space ID.

Creates a new post on the Workvivo activity feed
- **delete_social_post**: This action is irreversible.

Permanently deletes a post from Workvivo
- **get_event_details**: Retrieves details for a specific calendar event
- **get_post_details**: Retrieves details for a specific social post
- **get_space_details**: Retrieves details for a specific collaboration space
- **get_employee_profile**: Retrieves profile details for a specific employee
- **list_company_events**: Lists upcoming events scheduled in Workvivo
- **list_workvivo_posts**: Lists social posts and activity on the Workvivo platform
- **list_collaboration_spaces**: Lists collaboration spaces (groups) in Workvivo
- **list_employees**: Lists employees registered in the Workvivo directory


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Workvivo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 posts on the company feed."

**🤖 AI Agent:**
> I found the 5 most recent posts: 1. 'Q1 Goals Achievement' by John Doe, 2. 'New Office Opening' by Jane Smith, 3. 'Welcome our New Hires' by HR, and 2 others. Which one would you like to see the comments for?

---

**👤 You:**
> "Find the profile for employee ID 'emp-123'."

**🤖 AI Agent:**
> Profile for emp-123: Name: Robert Brown, Title: Senior Software Engineer, Department: Engineering, Email: robert@example.com. Would you like me to see which spaces he belongs to?

---

**👤 You:**
> "What are the details for the 'Town Hall' event today?"

**🤖 AI Agent:**
> Event 'Monthly Town Hall' (ID: ev-999): Starts at 03:00 PM UTC, Location: Main Auditorium / Zoom. Description: Q1 strategy update and open Q&A with the CEO. No agenda attachments found.


## Installation & Usage

To install and use the **Workvivo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/workvivo](https://vinkius.com/mcp/workvivo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
