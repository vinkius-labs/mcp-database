# Common Room MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/common-room)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/common-room-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/common-room-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Enable your AI agent to manage community contacts, segments, and activities via the Common Room API.

## Description
Connect your AI assistant to **Common Room**, the intelligent community growth platform that helps organizations find and build relationships with community members.

### What you can do

- **Contact Search** — Find community members by email, name, or external identity across connected platforms.
- **Segment Management** — List all segments, view member counts, and add or remove contacts from specific cohorts.
- **Activity Tracking** — Retrieve activity feeds to understand engagement patterns and identify key contributors.

### How it works

1. Add the Common Room integration to your AI toolset.
2. Provide your API Token (found under Settings > API Tokens).
3. Manage your community data via natural language commands.

### Who is this for?

- **Community Managers** — Quickly find and segment members without navigating the full dashboard.
- **DevRel Teams** — Identify top contributors and track engagement across channels from chat.
- **Growth Teams** — Build targeted segments and monitor community signal data in real time.


## Available Tools
- **add_contact_to_segment**: Manually add a contact to a specific segment
- **get_contact_by_email**: Retrieve detailed information about a member by their email
- **get_contact_tags**: Get tags associated with a specific member
- **get_organization_details**: Retrieve details of a specific organization
- **get_segment_status**: Retrieve status and member count for a specific segment
- **list_activity_types**: Retrieve a list of supported activity types in Common Room
- **list_segment_members**: List contacts that belong to a specific segment
- **list_segments**: Retrieve a list of all segments in Common Room
- **search_contacts**: Search for contacts/members in your Common Room
- **search_organizations**: Search for organizations in Common Room


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Common Room** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the member with email 'dev@example.com'."

**🤖 AI Agent:**
> Found member 'Alex Chen' (dev@example.com). They are in 2 segments: 'Top Contributors' and 'Beta Testers'. Last activity: GitHub PR merged 2 days ago.

---

**👤 You:**
> "Show me all segments and their member counts."

**🤖 AI Agent:**
> Your Common Room has 5 segments:
1. 'Top Contributors' — 128 members
2. 'Beta Testers' — 45 members
3. 'Enterprise Leads' — 312 members
4. 'New This Month' — 67 members
5. 'Churned' — 23 members
Would you like to explore any of these?

---

**👤 You:**
> "Add 'Alex Chen' to the 'Enterprise Leads' segment."

**🤖 AI Agent:**
> Successfully added 'Alex Chen' to the 'Enterprise Leads' segment. They are now in 3 segments total.


## Installation & Usage

To install and use the **Common Room** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/common-room](https://vinkius.com/mcp/common-room)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
