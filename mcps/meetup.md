# Meetup MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/meetup)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/meetup-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/meetup-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Manage your Meetup groups — audit upcoming events, members, and details via AI.

## Description
Empower your AI agent to orchestrate your entire community ecosystem with **Meetup**, the world's most trusted platform for finding and building local communities. By connecting Meetup to your agent, you transform complex group management into a natural conversation. Your agent can instantly list upcoming events, audit group memberships, and retrieve detailed event metadata without you ever touching a dashboard. Whether you are a community organizer or a frequent attendee, your agent acts as a real-time community coordinator, ensuring your event calendar is always monitored and your community reach is quantified.

### What you can do

- **Event Auditing** — List all upcoming events for any group and retrieve detailed metadata, including times and event URLs.
- **Group Oversight** — Search for new groups by keyword and monitor community distribution across your interests.
- **Member Administration** — Query member lists for your groups to stay on top of your community growth and participation.
- **Event Intelligence** — Retrieve full descriptions and details for specific events to ensure organizational alignment.
- **Discovery Monitoring** — Browse and identify new community opportunities through high-speed keyword search.

### How it works

1. Subscribe to this server
2. Enter your Meetup Access Token
3. Start managing your community through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Community Organizers** — monitor event signups and member growth straight from your workflow.
- **Marketing Leads** — verify if new events have been correctly published and described for maximum reach.
- **Networking Professionals** — perform rapid audits of local groups and identify relevant events without manual searching.
- **Operations Leads** — automate community querying to orchestrate cross-functional outreach teams smoothly.


## Available Tools
- **get_event**: Get details for a specific event
- **get_me**: Get authenticated user info from Meetup
- **list_group_members**: List members of a Meetup group
- **list_upcoming_events**: List upcoming events for a Meetup group
- **search_groups**: Search for Meetup groups by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meetup** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List upcoming events for the 'ny-tech' group."

**🤖 AI Agent:**
> I've retrieved the upcoming events for ny-tech. You have 3 events scheduled, including 'AI in 2024' and 'Web Dev Night'. Would you like the links for any of them?

---

**👤 You:**
> "Show me the member list for group 'london-data-science'."

**🤖 AI Agent:**
> I've found the membership list. There are currently 10 recent members visible, including 'Marcus R.' and 'Jane Doe'. Would you like their full profile details?

---

**👤 You:**
> "Search for groups about 'Machine Learning'."

**🤖 AI Agent:**
> I've identified several groups for 'Machine Learning'. Top matches include 'ML Experts London' and 'Data AI Community'. Which one would you like to explore?


## Installation & Usage

To install and use the **Meetup** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meetup](https://vinkius.com/mcp/meetup)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
